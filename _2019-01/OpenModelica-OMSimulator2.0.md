---
title: OMSimulator 2.0 final release with SSP
author: "Lennart Ochel and Adeel Asghar ([Open Source Modelica Consortium](https://openmodelica.org/))"
category: "vendor"
---

OMSimulator 2.0 provides a co-simulation and simulation environment for FMUs. The OMSimulator 2.0 final release is part of OpenModelica 1.13.2 and supports both ordinary signal connections and TLM (transmission line modelling) connections. Composite model structure and parameterization are stored according to the SSP standard, also allowing some extensions, e.g. bus connections. The figure shows the simulation of a composite FMI model.

![OMSimulator and OMEdit](https://openmodelica.github.io/OpenModelica-Resources/images/2019-OpenModelica-OMSimulator.png)

The following are highlights of OMSimulator 2.0:

* Efficient simulation of composite models based on model exchange and co-simulation FMUs
* Graphical composition of FMUs and visualization of simulation results
* Scripting interface, e.g. Python and Lua.
* Distributed simulations utilizing TLM master algorithm
* Increased numerical stability during co-simulation in various applications due to TLM connectors
* SSP (System Structure and Parameterization) support for composite models
* Modeling bus connections