---
title: OpenModelica 1.23
author: "Adeel Asghar, Francesco Casella [Open Source Modelica Consortium](https://www.openmodelica.org/)"
category: "vendor"
---

Version 1.23.0 of OpenModelica was released on 6 June 2024. It has many improvements and bug fixes compared to 1.22.3 (1.22.4 for Linux),
plus some new useful features, in particular regarding the OMEdit GUI and the FMI export feature. Version 1.23.1 is a minor release with fixes to OMEdit and omc to avoid crashes.

Real parameter values returned by the front-end when flattening models often had bad rounding, such as `499.99999999999` instead of `500` or `1.00000000000012` instead of `1.0`.
Also, bad rounding used to plague parameter values with unit conversions driven by `displayUnit` attributes in the OMEdit GUI.
In some cases, very long decimal outputs such as `1200000000.0` were displayed, instead of the more easily understood `1.2e9`.
This issue of proper rounding of decimal numbers was tackled systematically and resolved thanks to rounding algorithms based on the [Ryu library](https://github.com/ulfjack/ryu).

The new front end has been further improved. The front end can now provide clean [BaseModelica](https://github.com/modelica/ModelicaSpecification/blob/MCP/0031/RationaleMCP/0031/ReadMe.md)
flat output from the command line; experimental array-preserving flat output can also be obtained.

Most of the work on the backend is still focused on developing the new backend. Two notable improvements are worth mentioning:
  - the non-standard `annotation(tearingSelect)` was deprecated and replaced by `annotation(__OpenModelica_tearingSelect)`
  - according to the [Modelica Language Specification Sect. 8.6](https://specification.modelica.org/maint/3.5/equations.html#initialization-initial-equation-and-initial-algorithm)
    parameters with no binding and no explicitly set value now cause the compilation to fail, see [#10386](https://github.com/OpenModelica/OpenModelica/issues/10386).
    This may cause some old models to fail during compilation, but it is the required behaviour by the specification, to guard against parameters that are accidentally left without a meaningful value.
    The fix is to provide the modifier for the parameters without bindings, or to add an explicit `start = 0` modifier in the library model.
  - Issues related to the replaceable components and classes in the parameters
    window.

The quality of the OMEdit GUI was further improved over the previous version 1.22.3, with about 55 issues fixed. Most of them are bug fixes, but there are also some new features,
  - Duplicate class feature now works correctly also when the class is duplicated in another scope [#5346](https://github.com/OpenModelica/OpenModelica/issues/5346)
  - Top-level model parameters can now be edited with the GUI [#4408](https://github.com/OpenModelica/OpenModelica/issues/4408)
  - Further optimization of the editor's response time when deleting components and adding/deleting connections [#11920](https://github.com/OpenModelica/OpenModelica/issues/11920)
  - All rounding issues in the GUI resolved [#8865](https://github.com/OpenModelica/OpenModelica/issues/8865)

The full 1.23.0 release notes are available [here](https://github.com/OpenModelica/OpenModelica/releases/tag/v1.23.0).

The next release 1.24.0 is planned to be released in Q4 2024. It should include further improvements to the GUI such as parameter editing in hierarchically structured model,
restructured Simulation Setup dialog, Rename feature with refactoring, faster editing of large models in OMEdit, etc. Further improvements in FMI 2.0.x export are also planned.
