---
title: FMPy - simulate FMUs in Python
author: Torsten Sommer ([Dassault Systémes](https://www.3ds.com/))
category: library
---

FMPy is a free Python library to simulate Functional Mock-up Units (FMUs) that...

- supports FMI 1.0 and 2.0
- supports Co-Simulation and Model Exchange
- runs on Windows, Linux and macOS
- has a graphical user interface
- compiles source code FMUs

It's developed at Dassault Syst&egrave;mes and released under the 3-clause BSD license.  

For more information on how to install FMPy and a short tutorial take a look at the [documentation](http://fmpy.readthedocs.io/en/latest/) and visit our [project on GitHub](https://github.com/CATIA-Systems/FMPy).

Changes since the last newsletter:

**v0.2.5 (2018-06-17)**

Improved handling of input signals

- input is now applied before initialization for co-simulation
- "time" column for input signals can now have an arbitrary name


**v0.2.4 (2018-05-22)**

- `NEW` Remaining FMI functions added
- `NEW` More options for command line interface
- `NEW` More elements added to SSP parser
- `NEW` Polished GUI
- `FIXED` No more warning when starting GUI


**v0.2.3 (2018-04-11)**

- `NEW` Allow simulation of extracted FMUs and pre-loaded model descriptions
- `NEW` Re-load an FMU in the GUI
- `NEW` Load start values from an FMU
- `NEW` Write changed start values back to the FMU
- `NEW` Table editor for 1-d and 2-d array variables
- `NEW` Handle events in input signals
- `NEW` Plot events
- `NEW` Regular time grid for model-exchange results
- `NEW` Apply start values in the model description
- `NEW` Debug and FMI logging on the command line and in the GUI
- `NEW` Log filtering by type and message in the GUI
- `FIXED` Logger callback for FMI 1.0
- `FIXED` Handling of `None` in setString()
- `FIXED` Handling of time events
- `FIXED` Conversion of Boolean start values
