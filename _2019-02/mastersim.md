---
title: "MasterSim: Open-source FMI Co-Simulation Master takes next development step"
author: "Andreas Nicolai, [TUD](https://bauklimatik-dresden.de)"
category: vendor
---

The co-simulation master tool *MasterSim* (https://bauklimatik-dresden.de/mastersim), 
has reached a new important milestone. The open-source development aims at creating a 
reference implementation, that gives developers of master tools and FMI slaves as 
transparant piece of code to check and optimize their own implementations. 
For that purpose it implements most modern co-simulation coupling algorithms 
(Gauss-Jacobi, Gauss-Seidel, Newton) and supports FMI standards 1 and 2, the 
rollback-feature of the latter being used for the iterative algorithms. As C/C++ implementation, 
it is implemented with performance in mind (performance evaluators are welcome to compare it to 
other simulation engines). The code is hosted on 
https://sourceforge.net/projects/mastersim, which also includes the documentation (wiki-pages). 
The simulation engine is complemented by the equally free post-processing software *PostProc 2*
(https://bauklimatik-dresden.de/postproc).

![MasterSim with PostProc](screenshot_mastersim_06_with_postproc.png)

In the newest release 0.7, MasterSim can already handle quite a lot of reference FMUs from the cross-check repository on all three supported platforms (Windows, Linux, Mac), and also includes the capability of importing csv-files with predefined time series as input to slave variables. The simulator itself is a command-line tool that reads text files (project and data files) and writes results in csv-format text files as well, which makes it very suitable to be used in scripted environments (and optimization tools). In the upcoming releases the user interface will be extended to hold a graphical representation and include graphical routining, and will exchange such systems via the SSP-standardized file formats.

