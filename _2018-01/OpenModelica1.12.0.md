---
title: OpenModelica 1.12.0 Release
author: "Peter Fritzson [Open Source Modelica Consortium](https://www.openmodelica.org/)"
category: "vendor"
---

OpenModelica is the most complete open-source Modelica-based cyber-physical mathematical modeling,
simulation and optimization environment intended for industrial and academic usage.
Its long-term development is supported by a non-profit organization – the Open Source Modelica Consortium [OSMC](https://www.openmodelica.org/)
with many company, institute, and university members.

![](https://openmodelica.github.io/OpenModelica-Resources/images/2017-3DAnimation-V6Engine.jpg)

The figure shows 3D visualization and animation using OpenModelica.

Below the main aspects are described of the [OpenModelica 1.12.0 release](https://openmodelica.org/doc/OpenModelicaUsersGuide/v1.12.0/) from October 2017 which is the most recent stable regular release.
Substantial work on improved stability, library coverage, and verification coverage has been done.

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

