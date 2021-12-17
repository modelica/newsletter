---
title: Modelica improvements in the forthcoming Simcenter Amesim 2020.2
authors: "Karim Besbes([Siemens Digital Industries Software](https://www.sw.siemens.com/ ))"
category: "vendor"
---


[Siemens Digital Industries Software](https://www.sw.siemens.com/ ) anounces a new feature in the Modelica Editor of Simcenter Amesim 2020.2 called **exposed variables selection** allowing users to conveniently tune the meaningfull variables to be exposed for the simulation phase.
Additional new capabilities include:
* A blackbox button
* An internal variables filter button

This buttons allow to quickly activate/deactivate user-defined filters. 

#### Exposed variables selection from the Modelica Editor
In Simcenter Amesim's built-in Modelica edition tool, when a model is compiled, by default all the component's parameters and variables are exposed for the simulation. However, it is usually usefull to reduce the number of exposed variables to a subset of meaningfull ones before simulating a model. Therefore two options in the toolbar now allow to define which parameters and variables will be visible in Simcenter Amesim once the Modelica component is compiled: a Black-box button and an internal variables filter button. Only the model's state variables and its runtime parameters will always be visible.

With the Black-box button you can hide all your internal variables, thus avoiding to reveal your intellectual property or know-how.

With the internal variables filter button you can write directly the pattern of the variables to be exposed in accordance with the GLOB patterns specification. For example if you type <i>name*</i> in the dedicated text field, all the variables beginning with <i>name</i> will be exposed for the simulation phase. If you type <i>x* y*</i>, all the internal variables beginning with <i>x</i> or <i>y</i> will be exposed.

See the below example showing how a Modelica model made with the BuildSysPro library has been filtered by using the following pattern: <i>ParoiNord*</i> <i>ParoiSud*</i>

![Example of exposed variables selection](Simcenter_Amesim_Modelica_Editor_20202_example.png 'Example of exposed variables selection')

For more information on Simcenter Amesim, please visit our [website](https://www.plm.automation.siemens.com/global/en/products/simcenter/simcenter-amesim.html).
