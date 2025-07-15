---
title: News from the MSL project
author: MAP-LIB
category: "association"
---

#### MSL version 3.2.3 Build 3 released

After approval by both the MAP-LIB members and the Modelica Association members, version 3.2.3 Build 3 of the Modelica Standard Library has been released.
This is the second maintenance release for MSL version 3.2.3 containing eight back-ported bug-fixes that were resolved during the development of the upcoming new major release MSL version 4.0.0. If you are a user or distributor of the MSL version 3.2.3 it is recommended to update to this new maintenance release.

The release notes and the Modelica package can be downloaded from [GitHub](https://github.com/modelica/ModelicaStandardLibrary/releases/tag/v3.2.3%2Bbuild.3).

#### Towards MSL version 4.0.0

The upcoming new major version 4.0.0 of the Modelica Standard Library will be the first new major version in ten years. This version will be based on the recent Modelica language standard version 3.4, i.e., the MSL finally can be upgraded to drop deprecated features and to utilize new features such as [synchronous language elements](https://specification.modelica.org/v3.4/Ch16.html), [getInstanceName](https://specification.modelica.org/v3.4/Ch3.html#getinstancename), [spatialDistribution](https://specification.modelica.org/v3.4/Ch3.html#spatialdistribution) or the [pure/impure](https://specification.modelica.org/v3.4/Ch12.html#pure-modelica-functions) function notation. Backward-compatibility is no longer given, but a tested conversion script will be provided such that MSL users and library developers can easily upgrade their packages to the new version. All deprecated functionality will be either replaced by new features or still be available in a new additional package of obsoleted classes.

Additionally, it is a major goal to further improve the overall quality of the MSL with respect to class naming and package structuring, conventions and style guide-lines, icons, documentation style and improved example models.

As usual, you can follow the development or even participate on [GitHub](https://github.com/modelica/ModelicaStandardLibrary) using the [MSL4.0.0](https://github.com/modelica/ModelicaStandardLibrary/milestone/4) milestone. New contributors are very welcome and requested to sign the [CLA](https://www.modelica.org/licenses/ModelicaAssociationCLA_1.1) of the Modelica Association.

It is planned to release an alpha version of the MSL version 4.0.0 to the public early next year and to have the final release available by Q2/2020.
