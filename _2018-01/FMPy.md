---
title: FMPy - simulate FMUs in Python
author: Torsten Sommer
category: library
---


## FMPy

FMPy is a free Python library to simulate Functional Mock-up Units (FMUs) that...

- supports FMI 1.0 and 2.0
- supports Co-Simulation and Model Exchange
- runs on Windows, Linux and macOS
- has a graphical user interface
- compiles source code FMUs

It's developed at Dassault Syst&egrave;mes and released under the 3-clause BSD license.  
For more information on how to install FMPy and a short tutorial take a look at the [documentation](http://fmpy.readthedocs.io/en/latest/).

You've found a problem or have a suggestion? Visit our [GitHub project](https://github.com/CATIA-Systems/FMPy) and open an issue.


### Simulate an FMU in the Graphical User Interface

![FMPy GUI](FMPy/Rectifier_GUI.png)


### Simulate an FMU in Python

```
>>> from fmpy import *
>>> fmu = 'Rectifier.fmu'
>>> dump(fmu)  # get information

Model Info

  FMI Version       2.0
  Model Name        Rectifier
  Description       Model Rectifier
  Platforms         win64
  Continuous States 4
  Event Indicators  6
  Variables         63
  Generation Tool   MapleSim (1267140/1267140/1267140)
  Generation Date   2017-10-04T12:07:10Z

Default Experiment

  Stop Time         0.1
  Step Size         1e-07

Variables (input, output)

Name                Causality          Start Value  Unit     Description
outputs             output        282.842712474619  V        Rectifier1.Capacitor1.v
>>> result = simulate_fmu(fmu)         # simulate the FMU
>>> from fmpy.util import plot_result  # import the plot function
>>> plot_result(result)                # plot the variables
```

![Rectifier Result](FMPy/Rectifier_result.png)


### Simulate an FMU on the command line

To get information about an FMU directly from the command line change to the folder where you've saved the
FMU and enter

```
fmpy info Rectifier.fmu
```

Simulate the FMU and plot the results

```
fmpy simulate Rectifier.fmu --show-plot
```

Get more information about the available options

```
fmpy --help
```


### Advanced Usage

To learn more about how to use FMPy in you own scripts take a look at the
[examples](https://github.com/CATIA-Systems/FMPy/tree/master/fmpy/examples).
