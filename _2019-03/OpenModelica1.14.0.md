---
title: OpenModelica 1.14.0 Release
author: "Peter Fritzson [Open Source Modelica Consortium](https://www.openmodelica.org/)"
category: "vendor"
---

OpenModelica is the most complete open-source Modelica-based cyber-physical mathematical modeling,
simulation and optimization environment intended for industrial and academic usage.
Its long-term development is supported by a non-profit organization – the Open Source Modelica Consortium [OSMC](https://www.openmodelica.org/)
with many company, institute, and university members.

![](https://openmodelica.github.io/OpenModelica-Resources/images/2015-OpenModelica-V6Engine-3x4-cropped-400x287.png)

The figure shows OpenModelica with a plot from a simulation of the V6Engine model.

The most dramatic enhancement in the 1.14.0 release is the of the OpenModelica Compiler New Frontend (NF), which on the average gives a factor of 10-20 speed improvement in the flattening phase of compilation. The new frontend is default in this release. See www.openmodelica.org for download.

The speed of the OMEdit GUI has only slightly increased in this version, since it is still dependent mostly on the old frontend. Further GUI speed increases are available in the coming OpenModelica.1.15.0.

Some highlights:

- Implementation of expandable connectors completed in NF.
- The New Frontend (NF) is on the average about 20 times faster on flattening.
- A new more efficient and more correct implementation of arrays and records.
- The FMI OMSimulator API calls are now also available in the OMC API functions.
- Added possibility to generate analytic Jacobians for linear strong components.
- Added output language options for linearization: matlab, python, julia.
- Unified Jacobian evaluation from DASSL and IDA integrators.
- Added result check for linear solvers Lis, Klu, Total Pivot and Umfpack if a residual function is available.
- Improved debug dumping.
- Improved warning for iteration variables.
- OMMatlab  - A complete implementation is now available.


OMEdit:

- Drag and drop for the text layer.
- Auto completion of class names, components and annotations.
- Improved duplication functionality for copying classes.
- Better handling of Compiler flags.
- Support for connectorSizing annotation
- Documentation is available [here](https://openmodelica.org/doc/OpenModelicaUsersGuide/latest/omedit.html)
- Autocomplete annotations.
- Support for Icon/Diagram map annotation
- Model copy paste functionality
- Reset OMEdit settings/options.
- Array plots update on re-simulation
- Support for connectorSizing annotation.
- Drag and drop class names to text layer in OMEdit
- OMPlot: Improved plotting e.g., top and bottom margins for better view, snap to curve etc.

OMSimulator/FMI Simulation:

- Improvements in error control and numeric stability 
- Added adaptive step-size control based on roll-back mechanism
- Improved handling of output/input derivatives
- Provide first order derivatives for all continuous outputs of lookup tables
- Fixed various C-API calls and scripting bindings (lua, python)
- Fixed some command line options
- Improved various error messages
- Fixed signal filter for result files
- New functionality to add cpu time to the results for each simulation component
- Improved FMI export from OpenModelica (further improvements ongoing)
