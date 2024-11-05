---
title: Simcenter Amesim 2410 released
author: "Bruno Loyer ([Siemens Digital Industries Software](https://www.sw.siemens.com/ ))"
category: "vendor"
---
[Siemens Digital Industries Software](https://www.sw.siemens.com/ ) is pleased to announce the recent release of **Simcenter&nbsp;Amesim&nbsp;2410** as part of its [system simulation solutions]( https://blogs.sw.siemens.com/simcenter/whats-new-in-simcenter-systems-2410/). This release brings remarkable performance improvements to the solver and code generation, which it combines advantageously with previous optimizations such as those related to so-called &ldquo;0-flow&rdquo; problems or to discontinuity handling in a co-simulation context. 
![](amesim_banner_2410.png)

## Accelerated simulations
While the original aim was to speed up the simulation of Pseudo-Two-Dimensional (P2D) battery models 
&mdash;&nbsp;achieved with a speedup factor of about&nbsp;9&nbsp;&mdash;, two <i>generic</i> solver enhancements 
have been implemented which have immediate tangible positive consequences on all kinds of &ldquo;large&rdquo; 
models, which includes **Simcenter&nbsp;Amesim** native models but notably also Modelica models and imported Model Exchange FMUs, as soon as the &mdash;&nbsp;default&nbsp;&mdash; variable step solver is selected. 
These enhancements are:

* A new heuristic for optimized calculations of Jacobian matrices,
* An interface with the industry-standard [SuiteSparse KLU library](https://github.com/DrTimothyAldenDavis/SuiteSparse/tree/dev/KLU ).

## Improved code generation for Modelica and imported FMUs
On top of that, the code generation performed behind the scenes when creating a Modelica 
model, importing an FMU, a pre-trained neural network ([ONNX](https://onnx.ai/ ) file) or a response surface, 
has been significantly upgraded to &ldquo;V2&rdquo;, featuring lightweight and more efficient code. 
For Modelica and FMI, the direct 
outcome is a more robust coupled simulation with &ldquo;large&rdquo; models (numerous inputs/outputs,
state variables, internal variables and/or parameters). For highly-hierachical Modelica
models, the result is outstanding with compilation and simulation times that compete with 100% Modelica-based tools,
for example with models coming from Lawrence Berkeley's open-source [Buildings Library v11.0.0](https://simulationresearch.lbl.gov/modelica/ ). 

![](amesim_modelica_2410.png)

## Fast-running exported co-simulation FMUs
Obviously, the above-mentioned solver improvements for native or hybridized **Simenceter&nbsp;Amesim** models are automatically reflected&nbsp;&mdash;&nbsp;<i>embedded</i>&nbsp;&mdash;&nbsp; in exported 1.0, 2.0 or 3.0 FMUs for co-simulation. Combined with the optimized discontinuity handling introduced in release 2304, the speedup is further maximized in this context since at each co-simulation &ldquo;rendez-vous&rdquo; point, the solver's current pace is kept unchanged whenever possible. A typical use case is when the **Simcenter&nbsp;Amesim** FMU is connected to a controller model whose outputs may have changed little or not at all during a co-simulation time step. 

For more information on **Simcenter&nbsp;Amesim**, please visit our [website](https://www.plm.automation.siemens.com/global/en/products/simcenter/simcenter-amesim.html ).
