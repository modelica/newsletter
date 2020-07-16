---
title: Simcenter Amesim 2020.2 released
authors: "Karim Besbes([Siemens Digital Industries Software](https://www.sw.siemens.com/ ))"
category: "vendor"
---


[Siemens Digital Industries Software](https://www.sw.siemens.com/ ) is proud to announce the 
recent release of Simcenter Amesim 2020.2. The key new feature on Modelica Editor being **the exposed variables selection from Modelica Editor**.  
Additional new capabilities include:
* Blackbox button
* Internal variables filter button


#### Exposed variables selection from Modelica Editor
On the Modelica editor of Simcenter Amesim, when a model is compiled, by default all the component's parameters and variables are exposed for the simulation. However, two options from the toolbar allow to define which parameters and variables are visible in Simcenter Amesim after the Modelica component is compiled: the Black-box button and the Filter button. Of course, some variables cannot be filtered which are the input and output variables, the state variables and the runtime option parameters.

With the Black-box button you can hide all the internal variables, useful for example for confidentiality issues with a customer.

With the filter button you can write directly the pattern of the variables you need to expose by following the GLOB patterns specification. For example if you type name* in the text field, all the variables beginning with "name" will be exposed
in Simcenter Amesim. If you type x* y*, all the internal variables beginning with the letter x or y will be
exposed.

As an example below a screenshot showing how a Modelica model coming from the BuildSysPro library has been filterd by using the following pattern: ParoiNord* ParoiSud*

![Example of exposed variables selection](Simcenter_Amesim_Modelica_Editor_20202_example.png 'Example of exposed variables selection')

For more information on Simcenter Amesim, please visit our [website](https://www.plm.automation.siemens.com/global/fr/products/simcenter/simcenter-amesim.html).
