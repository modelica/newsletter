---
title: Electric Power Systems Library
author: "Dr. Clément Coïc  ([Dassault Systèmes Deutschland GmbH](https://www.3ds.com/))"
category: "library"
---


The Electric Power Systems Library (EPSL) is intended to assist the process of designing electrical power systems. It enables modeling Alternate Current (AC) and Direct Current (DC) as well as combined AC/DC (hybrid) networks found e.g. in More Electrical Aircrafts. Due to the use of a phasor based description, it enables fast simulation of AC systems, with performance basically independent of the AC system's frequency. The EPSL covers the key components of an electrical power system at different levels of detail. The architectural mode corresponds to "simple" phasor theory resulting in a quasi-static description of the system. The functional level of detail uses dynamic phasors to cover dynamic effects in the models. The modeling mode can currently be switched on a per-component basis via a parameter.
Additionally, the EPSL enables the description of harmonics of the fundamental AC frequency, which can be either constant or variable. Currently the AC components are either single or three-phased, whereas other phase numbers would be straight-forward to be added due to the generic modeling approach of components.
As an example, part of a generic aircraft electric power system architecture, proposed and studied within the MOET european project [MOET06], is modeled using EPSL in Dymola.
The power generation is realized thanks to the aircraft engines connected directly to Variable Frequency Starter Generators. The VFSGs convert the mechanical power into electrical power. The electrical power is then distributed to the consumers through High Voltage AC bus bar and DC bus bars.
Typical loads on the system are, for example: Environmental Control System (ECS), Electro-Mechanical Actuators (EMA), Wing Icing Protection System.
 
![](EPSL-MOET.png)

This architecture considers a large aircraft with four engines. The circuit associated to the first generator is illustrated in the figure above.

 [MOET06]	MOET Consortium Partners, More Open Electrical Technologies - Technical Report, 2006.
