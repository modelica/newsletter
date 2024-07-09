---
title: Process Systems Library – Dynamic Simulation of Power-to-X Processes
author: "Yann Pellny ([TLK Energy GmbH](https://tlk-energy.de/))"
category: "library"
---

For the past 5 years, TLK Energy has been developing a flexible and powerful Modelica library for process engineering. It has gone through several stages of development, from using Multiflash from KBC to calculate physical properties, to a completely new approach in calculating the state variables of the medium, to a stand-alone, affordable library. Instead of the usual calculation method using equilibrium states, phase properties are calculated separately, which offers more possibilities for parameterization. This makes it possible to simulate processes that were previously difficult to implement. Now the Process Systems Library (PSL) enables the simulation of many Power-to-X processes, from water electrolysis and carbon capture to synthesizing complex chemicals like methane or methanol. 
#### Example model: PEM Electrolyzer stack cooling
PEM electrolysis is highly efficient for hydrogen production, but to ensure optimal performance, the stack must be properly cooled. Reusing the waste heat can enhance the energy efficiency of the entire system.
 
During the electrolysis of water to hydrogen, waste heat needs to be removed for efficient operation. Many PEM stack manufacturers specify a maximum temperature rise (ΔTmax) between the incoming and outgoing reactant streams. Exceeding ΔTmax reduces the stack's lifespan and compromises system economics.

![system] (PSL-Power-to-X_system.jpg "system")

Adjusting the incoming mass flow controls the temperature rise, ensuring ΔTmax is not exceeded. Beyond a certain water mass flow, hydrogen production remains constant, but increased water flow enhances stack cooling. Minimizing pump power consumption involves keeping the mass flow as low as possible while maintaining ΔTmax.

A suitable control strategy helps maintain this optimal temperature rise dynamically. The PSL provides a simulation-ready example model that accounts for all these parameters, aiding in developing an appropriate operation for individual applications.

If you are wondering if PSL is suitable for your process and would like to know more or get a trial license, please contact us: [info@tlk-energy.de](mailto:info@tlk-energy.de)
