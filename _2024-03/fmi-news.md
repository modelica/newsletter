---
title: FMI news
author: MAP FMI
category: association
---

{::options parse_block_html="true" /}

![FMI](FMI.png)

#### First FMI Advisory Committee meetting

After the clarification of the FMI Project membership roles, the FMI Project hosted the first FMI Advisory Committee meeting on Nov 5, 2025.
We received very valuable feedback, ideas, and feature requests.
Thanks to the 70 participants for their contributions and participation!
(Participating Companies: Akkodis, Ansys, AVL, Beckhoff, Boeing, Bosch, Claytex, COMSOL, Dassault Systemes, dSPACE, EKS INTEC, GM Motorsports, KEB, Knorr Bremse, LBL, LTX, MachineWare, MapleSoft, Mathworks, Modelbased Cloud, Modelon, NVIDIA, PMSF, Principia MBS, Renault, Samares Engineering, Siemens, Synopsys, Volkswagen, Volvo Autonomous Solutions)

Some of the topics that were discussed:

* Support for new targets such as aarch64-linux in FMI 2.0 (already possible in FMI 2.0.4)
* Security aspects in the exchange of FMUs
* Memory safety requirements for FMUs
* Increase visibility of FMI in the US
* Improve recommendations on the use of FMU checkers (https://fmi-standard.org/validation/) 
* Using of the FMI for optimization, enhance support for partial derivatives
* Improve parameterization of FMUs
* Interoperability of Open-USD and FMI
* GPU support of FMUs (especially efficient data exchange)

These will be discussed in more detail in the FMI design group and actions will be derived. Stay tuned!

#### Maintenance releases FMI 3.0.2 and FMI 2.0.5: release process ongoing

The FMI project is preparing the maintenance releases FMI 2.0.5 and FMI 3.0.2.
Currently an inspection period is running for the release candidates, which you can find [on GitHub](https://github.com/modelica/fmi-standard/releases) together with a summary of changes.
In case of any findings, please [open an issue](https://github.com/modelica/fmi-standard/issues) as soon as possible.

#### Examples of Synchronous Clocked FMUs available

As more and more modelling and simulation tools extend their support for FMI 3.0, advanced features such as synchronous clocks get more into the focus. 
Thanks to Cláudio Gomes for providing an [instructive example](https://github.com/clagms/synchronous-clock-fmus) with several FMUs that can be used to understand the concept and to validate the Synchronous Clock support in importing tools. 
It has already been tested successfully in Altair Activate by Masoud Najafi.

![Synchronous-clocks](Synchronous-clocks.png)

#### FMI Layered Standard for for Network Communication (FMI-LS-BUS) 

The version v1.0.0 for CAN, CAN FD, CAN XL is in beta testing currently, and will be demonstrated at the International ASAM Conference in Munich in December.
In parallel we made progress on the Flexray support and are happy that we could tag [v1.1.0-alpha.1](https://github.com/modelica/fmi-ls-bus/releases/tag/v1.1.0-alpha.1).
Thanks to all contributors and stay tuned.

![FMI-LS-BUS-Roadmap](1730807979224.jpg)

#### FMI Design Face2Face Meeting in Munich Dec 2-3 2024

AVL will host a face-2-face in Munich at the beginning of December.
We will work on layered standards to the FMI standard and future improvements.

#### ASAM Conference in Munich Dec 4-5 2024

The FMI Project will present "FMI, Layered Standards and ASAM Standards - Enabling seamless SiL simulation of Virtual ECUs" at the coming International ASAM Conference in Munich. 
You can also meet us at the Modelica Association booth there.

We present three new Layered Standards for simulating virtual ECUs with FMI 3.0:

- [FMI-LS-XCP](https://github.com/modelica/fmi-ls-xcp) for measurement & calibration with XCP
- [FMI-LS-BUS](https://github.com/modelica/fmi-ls-bus) for simulation of network communication with CAN (FD, XL), FlexRay, Ethernet, LIN
- [FMI-LS-STRUCT](https://github.com/modelica/fmi-ls-struct) for structured entities like lookup tables

A demo from tool vendors (Akkodis, Altair, AVL, Bosch, dSPACE, PMSF, SYNOPSYS) illustrates the interoperability of these layered standards.

Looking forward to meet you in Munich.
More information on the conference on https://www.asam.net/conferences-events/detail/asam-international-conference-2024/.

![ASAM-Conference](asam-conference.jpg)

#### 16th Internation Modelica and _FMI_ Conference!

We are are happy to invite you to the coming [16th International Modelica & FMI Conference](https://modelica.org/events/modelica2025/) in Lucerne, where the importance of FMI is now also reflected in the conference title.

#### Other Resources and Discussion Forums for FMI related Questions

* Join the [LinkedIn FMI community](https://www.linkedin.com/groups/7477473/) to get the latest news on FMI, FMI supporting tools and discussions within the user community.
* Ask technical questions and discuss topics on the usage of FMI on [Stackoverflow tagged "FMI"](https://stackoverflow.com/questions/tagged/fmi).
* Report problems of the standard itself or suggestions for new features in form of issues on [fmi-standard.org](https://github.com/modelica/fmi-standard/issues).
