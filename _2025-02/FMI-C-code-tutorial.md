---
title: "FMI Import & Export using C Code Tutorial at the 16th International Modelica & FMI Conference"
author: "Torsten Sommer ([Dassault Systèmes](https://www.3ds.com))"
category: "conference"
---

![FMI Tutorial](FMI-tutorial-logo.png "FMI Tutorial"){:width="620px"}

**Time:** Monday, 08/Sep/2025, 1:30pm--4:45pm (including 30min coffee break)

We are happy to announce that there will be an extensive [FMI](https://fmi-standard.org/) tutorial at the upcoming [16th International Modelica & FMI Conference](https://modelica.org/events/modelica2025/).

In this tutorial we show how to write a simple FMI 3.0 implementation for a Co-Simulation FMU in C code. Starting with a minimalistic code framework we explain the implementation of all required functions and give best-practice recommendations on implementing error handling. The first part of the tutorial session is completed by building the FMU and simulating it in an FMI master program.

Next we present the steps on how to import an FMU into a software. Again, focus lies on implementation of the necessary functions and implementation of robust error handling. The FMU created in the first part is imported and run through a prepared simulation loop. Using the debugger we follow the function calls and develop an understanding of how the FMI master interacts with the FMU and how data is being exchanged.

We show how to build the FMU and the master program using platform-specific compiler tool chains. Participants can use their own development environment or use a prepared online compiler and development environment.
