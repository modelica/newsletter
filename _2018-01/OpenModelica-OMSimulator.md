---
title: OMSimulator 2.0 with FMI Composition Beta1 Release
author: "Lennart Ochel and Adeel Asghar ([Open Source Modelica Consortium](https://openmodelica.org/))"
category: "vendor"
---

OMSimulator is a rather new tool in the OpenModelica tool suite and provides a co-simulation and simulation environment for FMUs. The OMSimulator 2.0 release will be part of OpenModelica 1.13.0 and supports both ordinary signal connections and TLM (transmission line modeling) connections.

![OMSimulator and OMEdit](https://openmodelica.github.io/OpenModelica-Resources/images/2018-OpenModelica-OMSimulator.png)

The following are highlights of OMSimulator 2.0:

* Efficient simulation of composite models based on model exchange and co-simulation FMUs
* 3D visualization of connected mechanical model components which can be FMUs, Modelica models, or co-simulated components accessed via wrappers in ADAMS, Simulink, Beast, or Modelica
* Graphical composition of FMUs and visualization of simulation results
* Scripting interface
* Distributed simulations utilizing TLM master algorithm
* Increased numerical stability during co-simulation in various applications due to TLM connectors
* SSP (System Structure and Parameterization) support for composite models

![OMEdit, TLM 3D view](https://openmodelica.github.io/OpenModelica-Resources/images/2018-OpenModelica-OMSimulator-TLM.jpg)
