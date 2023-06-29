---
title: OpenModelica 1.21.0
author: "Francesco Casella, Adeel Asghar [Open Source Modelica Consortium](https://www.openmodelica.org/)"
category: "vendor"
---

Version 1.21.0 of OpenModelica was released on Apr 18 2023, with the goal of getting the release schedule back to the originally planned
two yearly releases, one in early spring after the OpenModelica Workshop, and one in autumn.

Version 1.21.0 does not contain major new features, but rather a number of incremental improvements
and bugfixes that substantially improved the software quality. Overall, [135 issues](https://github.com/OpenModelica/OpenModelica/issues?q=is%3Aissue+milestone%3A1.21.0+is%3Aclosed)
were addressed. 

Version 1.21.0 also allows to turn on the new instance-based API from the Tools | Options menu of OMEdit. This enables the GUI
to use the new frontend to get updated and correct information for rendering features such as conditional connectors,
parameter-depending dialog settings, parameter setting in replaceable classes, etc. It is also much faster than the previous
infrastructure, resulting in an improved user experience. If you are interested in experimenting
with this feature, we suggest to use the latest 1.22.0-dev nightly build, since a lot of further improvements and fixes were
applied since the release. We plan on making the new instance-based API the default choice with the forthcoming 1.22.0 release,
scheduled for Q4 2023.

The full 1.21.0 release notes are available [here](https://github.com/OpenModelica/OpenModelica/releases/tag/v1.21.0).
