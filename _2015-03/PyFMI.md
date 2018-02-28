---
layout: default
title: "PyFMI 2.2"
author: Maria Henningsson (Modelon)
category: vendor
---
![Jmodelica](https://www.modelica.org/publications/newsletters/2015-1/images/PyFMI_picture.png)

We are happy to announce the release of PyFMI 2.2! PyFMI comes with support for working with FMI 1.0 and 2.0, both Model-Exchange and Co-Simulation. With PyFMI’s companion package Assimulo, FMUs are simulated with a wide range of quality integration algorithms, including CVode from the Sundials suite, Radau and Implicit/Explicit Euler.

For this release we are glad to announce the following highlights:

-  Compressed sparse calculation of the Jacobian that can substantially increase simulation performance
-  Sensitivity computation with respect to model parameters (requires that model parameter is set to an input)
-  Support for Python 3

For more information and documentation, see the [PyFMI web page](http://www.jmodelica.org/page/4924).