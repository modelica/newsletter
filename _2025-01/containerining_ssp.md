---
title: Containerizing SSP
author: "Dag Brück ([Dassault Systèmes AB](https://www.dymola.com/))"
category: "education"
---

![DC Motor variants](https://github.com/user-attachments/assets/6b4cc490-c437-4d93-b454-dffbcd152d90)

SSP means [System Structure and Parameterization](https://ssp-standard.org/), a relatively new standard for storing simulation models, parameter sets, and documentation.
Containerizing an SSP file is the new thing around town.
By that I mean converting a system described with SSP to a free-standing Functional Mockup Unit (FMU), which is a great benefit for tools that do not support SSP (yet).

Dymola supports import of SSP and export of FMUs (big news, huh?). Would it be possible to extend Dymola with SSP containerization?

#### Simple containerization
Actually, that is pretty trivial to do using existing functionality, because `importSSP` returns the name of the Modelica model generated for the "root" system defined by the SSP.
So we can use that to export an FMU.

```
m = importSSP("DC-Motor2023.ssp", silentSave=true);
translateModelFMU(m, false, "DC_Motor", "2", "cs", false, 1);
```

#### Containerizing a parameterized model
The next natural step is to apply an additional parameter set to our model, and then export it as an FMU with modified parameters encapsulated in the FMU.
Here we make an experiment by increasing the inductance of the electrical machine, where the data is stored in a CSV file.
The command `importSSV` takes a parameter file in SSV or CSV format, and a model to apply those parameters to.

```
m_alt2 = importSSV("DC_Motor_Alt2.csv", m);
translateModelFMU(m_alt2, false, "DC_Motor_Alt", "2", "cs", false, 1);
```

In Modelica we use the common idiom of extending from the base model while appying modifed parameters in the extends-clause.

#### Running a comparison
To run the simulation we can import the two FMUs, drop them into a model (called Unnamed, this step is not shown) and simulate.

```
importFMU("DC_Motor.fmu", true, false, false, "", fill("",0), "DC_Motor_fmu");
importFMU("DC_Motor_Alt.fmu", true, false, false, "", fill("",0), "DC_Motor_Alt_fmu");
simulateModel("Unnamed", resultFile="Unnamed");
```

The result demonstrates that increasing the inductance from 1 mH to 5 mH softens the motor torque.
