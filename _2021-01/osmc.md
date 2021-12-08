---
title: OpenModelica 1.17.0 released
author: "[Francesco Casella](https://openmodelica.org/)"
category: "vendor"
---
We are happy to announce that OpenModelica 1.17.0 was released on 23 March 2021.

#### New Frontend

After three years of development work, the new frontend is now used by default by all the tools of the OpenModelica suite, 
providing faster code generation time and improved coverage of the Modelica language features. 

#### Improved user experience under Windows

The Windows version of the OMEdit GUI was substantially improved in terms of graphics rendering and GUI responsiveness. The use
of clang instead of gcc to compile C code also provides much shorter compilation time of models.

#### Support of MSL 4.0.0

OpenModelica and OMEdit now support Modelica Standard Library 3.2.3 and 4.0.0. There are currently 
two main limitations with MSL 4.0.0: clocked components are still not fully reliable, and automatic conversion scripts are not
yet available. We plan to resolve these two issues with the next release 1.18.0, due this fall.

The tool can be downloaded from the [OpenModelica website](https://openmodelica.org). For further details, please check the [1.17.0 Release Notes](https://trac.openmodelica.org/OpenModelica/wiki/ReleaseNotes/1.17.0)
