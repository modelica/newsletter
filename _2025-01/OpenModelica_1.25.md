---
title: OpenModelica 1.25.0
author: "Adeel Asghar, Francesco Casella [Open Source Modelica Consortium](https://www.openmodelica.org/)"
category: "vendor"
---

OpenModelica 1.25.0 will be released late March 2025. It will be regular early-spring release of OpenModelica.

Main highlights: OMEdit now supports **hierarchical parameter editing** in structured models, a **Reload package** feature, and an **Open Class in text view** feature.

## OpenModelica Compiler (OMC)

The new front end has been further improved with [15+ issues solved](https://github.com/OpenModelica/OpenModelica/issues?q=is%3Aissue%20milestone%3A1.25.0%20label%3ACOMP%2FOMC%2FFrontend%20state%3Aclosed%20-reason%3Anot-planned).
[Two fixes](https://github.com/OpenModelica/OpenModelica/issues?q=is%3Aclosed%20is%3Aissue%20milestone%3A1.25.0%20label%3A%22COMP%2FBase%20Modelica%22%20) regarding the new experimental
[Base Modelica flat output](https://openmodelica.org/doc/OpenModelicaUsersGuide/latest/basemodelica.html#flattening-models-to-basemodelica).

Regarding backend work, [5 issues](https://github.com/OpenModelica/OpenModelica/issues?q=state%3Aclosed%20milestone%3A1.25.0%20label%3A%22COMP%2FOMC%2FBackend%22%20-reason%3Anot-planned%20) were fixed in the currently used
backend. Additionally, [15 issues](https://github.com/OpenModelica/OpenModelica/issues?q=state%3Aclosed%20milestone%3A1.25.0%20label%3A%22COMP%2FOMC%2FNew%20Backend%22%20-reason%3Anot-planned) were address in the new backend,
which is still under development and experimentally available with the [`--newBackend`](https://openmodelica.org/doc/OpenModelicaUsersGuide/latest/omchelptext.html#omcflag-newbackend) compiler flag.

Regarding the C runtime, [several issues](https://github.com/OpenModelica/OpenModelica/issues?q=is%3Aissue%20milestone%3A1.25.0%20label%3ACOMP%2FSimRT%2FC%20state%3Aclosed%20-reason%3Anot-planned%20) were addressed. 

A new experimental feature, the Newton Diagnostics, was added to the C runtime. This feature can be activated by the simulation flag
[`-lv=LOG_NEWTON_DIAGNOSTICS`](https://openmodelica.org/doc/OpenModelicaUsersGuide/latest/simulationflags.html#simflag-lv); this computes and displays a ranking of the most likely start attributes responsible for the
failure of Newton-Raphson iterations on nonlinear implicit systems during initialization. As such, it can be an invaluable tool for troubleshooting initialization failures due to convergence issues caused by badly
chosen start attributes. For more details see the [paper](https://doi.org/10.1016/j.amc.2021.125991) by F. Casella and B. Bachmann on this topic (here is an open-access [preprint](https://arxiv.org/abs/1911.12433) on ArXiv)
and the [presentation](https://openmodelica.org/images/M_images/OpenModelicaWorkshop_2025/2025-02-03_Newton_Diagnostics.pdf) at the 2025 OpenModelica Workshop for more details. Please note that residual scaling
is still not implemented, so this feature is not yet fully operational when applied to systems of equations that are badly scaled due to the use of SI units.

## Graphical Editor OMEdit

OMEdit 1.25.0 provides several, long awaited-for features.

The first is hierarchical editing of model parameters [#2891](https://github.com/OpenModelica/OpenModelica/issues/2891): you can now change parameters not only for top-level components, but also for its sub-components.
This feature is available by right-clicking over component icons and selecting Show Element; this can be done recursively to set parameters of sub-sub-components, etc..
Replaceable components and classes can be handled in the same way. Previously, this was only possible by switching to the textual input mode and by manually adding the corresponding nested modifiers and redeclare clauses
to the top-level component instances.

The Reload feature was implemented [#5664](https://github.com/OpenModelica/OpenModelica/issues/5664): if you right-click on a top-level package, the whole package is unloaded from memory and reloaded from the file system,
_while preserving the status of the already opened sub-packages in the Library browser_. Previously, you had to first select Unload, then re-open the package,
and then navigate again through the sub-package hierarchy to reach the model(s) of your interest. This feature is very convenient when working with multiple Modelica tools in parallel,
or when editing some parts of a library with textual editors, because it allows to update the loaded package to the updated version on the file system with a single mouse click.

When browsing the code of a class in the textual view, it is now possible to open any class mentioned in the source code by just right-clicking on it and selecting Open Class,
or just by the ctrl-click shortcut [#8854](https://github.com/OpenModelica/OpenModelica/issues/8854).

It is now possible to select a part of a model diagram by dragging a selection window, then copy and paste all the selected components either in the same model,
or into a new model [#12687](https://github.com/OpenModelica/OpenModelica/issues/12687).

OMEdit now automatically adds the `each` prefix when providing scalar parameter values to parameter arrays,
avoiding the common error of forgetting to add it manually [#13636](https://github.com/OpenModelica/OpenModelica/issues/13636).

The new instance-based infrastructure of OMEdit is now fully mature and far superior to the old graphical editing mode from all points of view.
Hence, starting from version 1.25.0, support of the old graphical editing mode is dropped [#13257](https://github.com/OpenModelica/OpenModelica/issues/13257).

Many OMEdit bugs were also fixed in this release. Overall, [40+ issues](https://github.com/OpenModelica/OpenModelica/issues?q=milestone%3A1.25.0%20state%3Aclosed%20label%3ACOMP%2FGUI%2FOMEdit%20-reason%3Anot-planned%20is%3Aissue%20) were addressed.

## FMI export

[Several issues](https://github.com/OpenModelica/OpenModelica/issues?q=milestone%3A1.25.0%20label%3ACOMP%2FFMI%20state%3Aclosed%20-reason%3Anot-planned) regarding FMI export were addressed.

A serious bug [#13582](https://github.com/OpenModelica/OpenModelica/issues/13582) affecting co-simulation FMUs using the CVODE stiff solver was identified.
It has been not yet fixed, but it should be fixed in the final 1.25.0 release, or in a patch 1.25.1 release.

## OMSimulator

OMSimulator focused on improving Model Exchange simulations. We analyzed multiple Modelica libraries, including MSL4, and addressed key issues in event handling and ODE solver implementation.
These enhancements increased coverage from ~50% to ~95% across several libraries.
The results were [presented](https://openmodelica.org/images/M_images/OpenModelicaWorkshop_2025/2025-02-03_OMSimulator.pdf) at the OpenModelica workshop in February 2025.
The latest stable release, OMSimulator 2.1.3, is available on GitHub or via pip `pip install OMSimulator`

## Next release

The next release is planned to be released in autumn 2025. It should include further improvements to the GUI such as a restructured Simulation Setup dialog, faster editing of large models in OMEdit, etc.
Further improvements in FMI 2.0.x export are also planned.
