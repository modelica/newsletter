---
title: Multi-Domain Drone Modeling with the New Open Source Drone Library (Free)
author: "Luigi Vanfretti [Rensselaer Polytechnic Institute](https://alsetlab.github.io)"
category: "library"
---
![Alt text](Dronepackage.png 'Drone Library')

Based on research responding to the growing need of simulation-based studies in Unmanned Aerial Vehicle (UAV) [1, 2], <code>the DroneLibrary</code>, aggregates and streamlines the authors's previous efforts in the area providing multi-domain models to represent each sub-system of drones.

This library contains examples of the quadcopter model at multiple levels of detail under different operating conditions. The component models are developed in a manner to easily replace them for different simulation applications, creating replaceable models that are easy to maintain with broad application scope.

![Alt text](DroneLib_Example1.png 'Drone Library')

Some of the key features are:
- Component models allowing the modeling of multi-copter configurations beyond the provided quadcopter examples.
- A number of configurations allowing to compare different electric power train designs.
- Numerous example models showing a variety of drone configurations, including popular consumer drones.
- Examples exploiting DLR's Visualization Library and the Modelica_DeviceDrivers Library for enhanced visualization and immersive user-interaction. 

The library has been developed in Dymola. The library was also tested with OpenModelica where currently the models pass checks but may not simulate, contributions increasing compatibility with OpenModelica are welcome as pull requestions online: [https://github.com/ALSETLab/Modelica-Drone-3D-FMI](https://github.com/ALSETLab/Modelica-Drone-3D-FMI).

[Click here to download the library](https://github.com/ALSETLab/Modelica-Drone-3D-FMI/releases).

References:

[1] M. Podlaski, et al (2020-10). “UAV Dynamic System Modeling and Visualization using Modelica and FMI”. In: VFS 76th Annu. Forum & Tech. Display. doi : 10 . 4050 / F - 0076 -
2020-16289., pp. 1058–1072. [Available online](https://www.researchgate.net/publication/344595743_UAV_Dynamics_and_Electric_Power_System_Modeling_and_Visualization_using_Modelica_and_FMI).

[2] M. Podlaski, et al (2021). “Towards a VR-Based Early Design Interaction for Electric Vertical Take-Off & Landing (eVTOL) Cyber-Physical Models”. In: 2021 NAFEMS World
Congr. NAFEMS. [Available online](https://www.researchgate.net/publication/372128766_Towards_VR-Based_Early_Design_Interaction_for_electric_Vertical_Take-Off_Landing_eVTOL_Cyber-Physical_Models).


