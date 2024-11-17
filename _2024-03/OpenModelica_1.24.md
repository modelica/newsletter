---
title: OpenModelica 1.24.0
author: "Adeel Asghar, Francesco Casella [Open Source Modelica Consortium](https://www.openmodelica.org/)"
category: "vendor"
---

Version 1.24.0 of OpenModelica was released on 9th October 2024. It has many improvements and bug fixes. Graphical Editor (OMEdit) was updated to support both Qt5 and Qt6.

#### OpenModelica Compiler (OMC)

The new front end has been further improved with about 25 issues solved, here is a [complete list](https://github.com/OpenModelica/OpenModelica/issues?q=is%3Aissue+milestone%3A1.24.0+label%3ACOMP%2FOMC%2FFrontend+is%3Aclosed+). [Nine of those issues](https://github.com/OpenModelica/OpenModelica/issues?q=is%3Aclosed+milestone%3A1.24.0+label%3A%22COMP%2FBase+Modelica%22+) regarded fixes to the new experimental [Base Modelica flat output](https://openmodelica.org/doc/OpenModelicaUsersGuide/latest/basemodelica.html#flattening-models-to-basemodelica).

A new compiler flag [--exposeLocalIOs](https://openmodelica.org/doc/OpenModelicaUsersGuide/latest/omchelptext.html#omcflag-exposelocalios) was added to automatically add the outputs of a model components to the outputs of an FMU, instead of only adding the top-level outputs. This can easily provide monitoring information in an FMU without the need of painstakingly bring all those outputs to the top level in the original Modelica model.

Besides [#12730](https://github.com/OpenModelica/OpenModelica/issues/12730), the work on the backend was mostly focused on developing the new backend, with [14 issues](https://github.com/OpenModelica/OpenModelica/issues?q=is%3Aclosed+milestone%3A1.24.0+label%3A%22COMP%2FOMC%2FNew+Backend%22+) being fixed. 

One [small fix](https://github.com/OpenModelica/OpenModelica/issues?q=is%3Aclosed+milestone%3A1.24.0+label%3ACOMP%2FOMC%2FRuntime) was made to the C runtime.

#### Graphical Editor (OMEdit)

The OMEdit source code was adapted to use both Qt5 and Qt6, see pull request [#12485](https://github.com/OpenModelica/OpenModelica/pull/12485).

The quality of the OMEdit GUI was further improved over the previous version 1.23.1, with about 15 issues fixed, see the
[complete list](https://github.com/OpenModelica/OpenModelica/issues?q=milestone%3A1.24.0+is%3Aclosed+label%3A%22COMP%2FGUI%2FInstBased+Interface%22%2CCOMP%2FGUI%2FOMEdit+). 

An important improvement regarding the usability of the GUI concerns the reaction time when editing diagrams, which used to be very slow when adding or removing components and connections in large models; these operations are now much faster, while changing parameters can still be quite slow. See [#11920](https://github.com/OpenModelica/OpenModelica/issues/11920) for more details.

The full 1.24.0 release notes are available [here](https://github.com/OpenModelica/OpenModelica/releases/tag/v1.24.0).

The next release 1.25.0 is planned to be released in January/February 2025, with a first beta release possibly before the end of the year. It should include further improvements to the GUI such as parameter editing in hierarchically structured model, restructured Simulation Setup dialog, rename feature with refactoring, faster editing of large models, etc. Further improvements in FMI 2.0.x export are also planned.
