---
title: OpenModelica 1.12.0 Release
author: "Peter Fritzson [Open Source Modelica Consortium](https://www.openmodelica.org/)"
category: "vendor"
---

OpenModelica is an open-source Modelica-based cyber-physical mathematical modeling,
simulation and optimization environment intended for industrial and academic usage.
Its long-term development is supported by a non-profit organization – the Open Source Modelica Consortium [OSMC](https://www.openmodelica.org/)
with many company, institute, and university members.

![](https://openmodelica.github.io/OpenModelica-Resources/images/2017-3DAnimation-V6Engine.jpg)

The figure shows 3D visualization and animation using OpenModelica.

Below the main aspects are described of the [OpenModelica 1.12.0 release](https://openmodelica.org/doc/OpenModelicaUsersGuide/v1.12.0/) from October 2017 which is the most recent stable regular release.
Substantial work on improved stability, library coverage, and verification coverage has been done.
An OpenModelica 1.13.0 Beta release is planned in April-2018.[see]((https://www.openmodelica.org/))

Summary of some of the most important improvements:

- A new (stand-alone) FMI- and TLM-based simulation tool OMSimulator 1.0, this first version for connected FMUs, TLM objects,
  Simulink models (via wrappers), Adams models (via wrappers), BEAST models (via wrappers), Modelica models
- Graphic configuration editing of composite models consisting of FMUs
- Increased library coverage including significantly increased verification coverage
- Graphical editing support for state machines and transitions
- An OMEdit HTML WYSIWYG Editor, e.g. useful for documentation
- Faster lookup processing, making some libraries faster to browse and compile
- Additional advanced visualization features for multibody animation
- Increased tool interoperability by addition of the ZeroMQ communications protocol
- Enhanced OMPython including linearization, now also working with Python 3
- Support for Linux RedHat/Fedora binary builds of OpenModelica
- Support for exporting the system of equations in GraphML (yEd) format for debugging

#### OpenModelica supports 3D visualization and animation in two ways

1. Built-in 3D animation and visualization in OMEdit of multi-body systems (since OpenModelica v1.11.0; see the [User's Guide](https://openmodelica.org/doc/OpenModelicaUsersGuide/v1.12.0/omedit.html#d-visualization) for instructions).
2. Visualization using third-party libraries such as the commercial DLR Visualization library.

<i>Visualization in OMEdit of Multi-Body Systems</i>

Below: An example 3D visualization and animation of an excavator (Courtesy TU Dresden).

![Excavator](https://openmodelica.github.io/OpenModelica-Resources/images/2017-3DAnimation-Excavator.png)

* This is a built-in feature of OMEdit to visualize and animate MSL-Multi-Body shapes
* Supports visualization and animation of simulation results
* Animation of geometric primitives and CAD-Files


<i>Visualization Using the External DLR Visualization Library</i>

Below: Visualization and animation of the DLR ROboMObil (Courtesy DLR).

![Robomobil](https://openmodelica.github.io/OpenModelica-Resources/images/2018-DLR-Visualization-3D-Robomobil.jpg)

The DLR visualization library supports the following:
* Advanced, model-integrated and vendor-unspecific visualization for Modelica models
* Offline, online and real-time animation
* Video-export function
* Commercial library, a feature reduced free Community Edition exists

#### OpenModelica Code Generators for Embedded Real-Time Code

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

#### Enhanced OMPython Including Control Design

OMPython is the Python scripting interface to the OpenModelica [tool suite](https://www.openmodelica.org/).
An Enhanced OMPython version has recently been developed, making it possible to perform control design,
model linearization, sensitivity analysis, etc. [UserGuide](https://www.openmodelica.org/doc/OpenModelicaUsersGuide/latest/ompython.html#enhanced-ompython-features)

![](closedloop.jpg)

Investigating closed loop eigenvalues

![](Seborg-Chemical.jpg)

Simulation of a Seborg chemical process reactor controlled by a PI controller
 
The enhanced OMPython is available in the OpenModelica 1.12.0 final release and later releases. Below some highlights are briefly mentioned.:

- Access to the whole OpenModelica scripting API
- Loading, compiling, and simulating models
- Operations on models such as linearization.
- Loading simulation results for analysis, plotting, etc.
- Parameter sweeps, e.g. sensitivity analysis.
- Control design.
