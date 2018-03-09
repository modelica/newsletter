---
title: OpenModelica Code Generators for Embedded Real-Time Code
author: "Martin Sjölund ([Open Source Modelica Consortium](https://openmodelica.org/))"
category: "vendor"
---

OpenModelica currently (as of v1.12.0) provides two flavors of code
generators for embedded real-time code:

A full-fledged OpenModelica-generated source-code FMU (Functional Mockup Unit) code generator:

* Can be used to cross-compile FMUs for platforms with more available memory.
* These platforms can map FMI inputs/outputs to analog/digital I/O in the importing FMI master.

A very simple experimental code generator generating a very small footprint statically linked
executable:

* Not an FMU because there is no OS, filesystem, or shared objects in microcontrollers.

Below is the [SBHS](http://vlabs.iitb.ac.in/sbhs/) (a teaching board using an ATmega16 microcontroller) running an OpenModelica-based
controller (the Arduino is based on the same microcontroller and is also supported in the [Modelica_DeviceDrivers](https://github.com/modelica/Modelica_DeviceDrivers) library):

![SBHS board](https://openmodelica.github.io/OpenModelica-Resources/images/2017-OM-real-time-controller-codegen-SHBS-Arduino.jpg)
