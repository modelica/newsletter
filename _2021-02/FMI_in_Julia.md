---
title: Announcing FMI.jl & FMIFlux.jl
author: "Lars Mikelsons"
category: "vendor"
---

![](fmijl_logo_640_320.png)  
The simulation ecosystem of the Julia programming language is rapidly growing. In order to bridge the gap between industrial use cases and methods and algorithms available in Julia, `FMI.jl` (https://github.com/ThummeTo/FMI.jl) is released.  
`FMI.jl` aims at the integration of FMI (https://fmi-standard.org/) into the Julia ecosystem by providing the possibility to load, parameterize and simulate FMUs.

![](fmifluxjl_logo_640_320.png)  
Combining physical and state-of-the-art data-driven modeling inside a single simulation tool used in industry is currently not possible in a convenient fashion. An extension to `FMI.jl` called `FMIFlux.jl` (https://github.com/ThummeTo/FMIFlux.jl) allows the integration of FMUs into neural network topologies to obtain a *NeuralFMU*.  
This structural combination of a black-box model commonly used in industry and a data-driven machine learning model combines the different advantages of both modeling approaches in a single Julia-based development environment. This allows for the usage of advanced data driven modeling techniques for physical effects that are difficult to model based on only first principles.
