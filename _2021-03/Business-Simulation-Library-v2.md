---
title: Business Simulation Library v2.0 released!
author: "Guido Wolf Reichert [BSL MANAGEMENT SUPPORT]"
category: "vendor"
---
The free Business Simulation Library (BSL) supports modeling & simulation of dynamical systems in the social sciences, e.g., business, economics, and ecology using the System Dynamics metaphor. Unlike the well known System Dynamics library the BSL makes use of *acausal* connectors so that mutiple flows will automatically add up when connected to a stock and mass balance requirements will not be violated when making connections across subsystems in a model. The *potential* variable within an acausal connection is used to transmit the amount contained in a connected stock making diagrams less cluttered and modeling faster\[LongDash]see the *word of mouth* interaction between potential customers and customers in the model diagram below, which is an example that ships with the library.

![Alt text](BSL-production-chain.png 'production chain')

The new release, while fixing some errors with regard to platform compatibility, mainly adds high-level classes for agile modeling of dynamical systems using an impact diagram like framework: Domain experts simply need to provide estimates for *polarity*, *strength*, and an (optional) *delay time* to specify the impact of one variable upon another, where the strength of impact is specified as a proportionality factor or an  elasticity coefficient (see the release notes [here](https://bsl-support.de/BusinessSimulation/BusinessSimulation.UsersGuide.ReleaseNotes.Version_2_0_0.html)).

The library was developed using Wolfram System Modeler and can be downloaded from its library store [here](https://www.wolfram.com/system-modeler/libraries/business-simulation/) or it can be downloaded from the developer's GitHub accound [here](https://github.com/bslMS/BusinessSimulation).
