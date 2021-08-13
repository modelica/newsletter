---
title: Simcenter Amesim 2021.1 released
authors: "Karim Besbes([Siemens Digital Industries Software](https://www.sw.siemens.com/ ))"
category: "vendor"
---


[Siemens Digital Industries Software](https://www.sw.siemens.com/ ) is proud to announce the 
recent release of [Simcenter Amesim 2021.1](https://www.youtube.com/watch?v=YNwLOHDF148&ab_channel=SiemensSoftware), as part of its system simulation solutions. Among the key features introduced in this release, we can highlight the Modelica related improvements below.

#### Modelica Editor 2021.1
Modelica Editor is an integrated development application dedicated to editing Modelica code. More than a tool to be used during the design and modeling phase of a Modelica model, Modelica Editor allows you to generate bridges between the acausal world of Modelica and the causal environment of Simcenter Amesim.

The improvements introduced in Modelica Editor 2021.1 since the last release are the following:
* Modelica Compiler (Modelon’s Optimica Compiler Toolkit) upgraded to version 1.24
* Semantic checker added in the toolbar to perform a syntax and symbolic analysis of the active model and ensure the balance between the equations and variables
* New Modelica package providing robust interfaces between the MSL fluid standard connectors and the **Thermal Hydraulic** submodels of Simcenter Amesim

This new Modelica package contains 2 different interfaces to consider the causalities of the Thermal Hydraulic submodels. With these interfaces, it is now possible to connect for instance a Modelica-based heat exchanger to a Simcenter Amesim native closed loop cooling system.

![Hybrid modelling example](Simcenter_Amesim_Modelica_Editor_20211_example.png 'Application example of Simcenter Amesim')

And thanks to the media property assistant provided in the **Thermal Hydraulic library**, the media used in Simcenter Amesim can be adjusted according to the properties described in Modelica, thus obtaining continuous thermodynamic properties between both worlds.

For more information on Simcenter Amesim, please visit our [website](https://www.plm.automation.siemens.com/global/fr/products/simcenter/simcenter-amesim.html).

