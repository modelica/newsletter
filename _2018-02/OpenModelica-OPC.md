---
title: Interactive Simulation in OpenModelica with OPC-UA
author: "Martin Sjölund ([Open Source Modelica Consortium](https://openmodelica.org/))"
category: "vendor"
---

Interactive simulation and interactive control of simulations is provided in OpenModelica 1.13.0 using
OPC-UA, which is an industry standard for industrial automation.

OPC-UA in OpenModelica:

* Controls simulations in real-time
* Changes inputs and state variables on the fly
* Performs interactive plotting
* More lightweight than controlling FMUs for your own simple applications

There are open source OPC-UA clients available in C++, Python, etc.

The video below shows an early prototype of the interactive plotting.

<video width="640" controls>
  <source src="https://openmodelica.github.io/OpenModelica-Resources/movies/interactive-simulation.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>
