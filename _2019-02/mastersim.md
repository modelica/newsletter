---
title: "MasterSim: Open-source FMI Co-Simulation Master takes next development step"
author: "Andreas Nicolai, [TUD](https://bauklimatik-dresden.de)"
category: vendor
---

The co-simulation master tool *MasterSim* (https://bauklimatik-dresden.de/mastersim) 
has reached a new important milestone - with key focus on standard compliance and ability to
run a larger number of cross-check FMUs. 

*MasterSim* is an open-source development that aims at creating a 
reference implementation, giving developers of master tools and FMI slaves a 
transparant implementation to check and optimize their own implementations. 
For that purpose several modern co-simulation coupling algorithms 
(Gauss-Jacobi, Gauss-Seidel, Newton) are implemented, and FMI versions 1 and 2 are supported. The 
rollback-feature of the latter is being used for the iterative algorithms. As C/C++ implementation, 
it is implemented with performance in mind (performance evaluators are welcome to compare it to 
other simulation engines). The code is hosted on 
https://sourceforge.net/projects/mastersim which also includes the documentation (wiki-pages). 
The simulation engine is complemented by the equally free post-processing software *PostProc 2*
(https://bauklimatik-dresden.de/postproc), which features run-time live updates of simulation progress.

![MasterSim with PostProc](screenshot_mastersim_06_with_postproc.png)

In the newest release 0.7, *MasterSim* can already handle quite a lot of reference FMUs from 
the cross-check repository on all three supported platforms (Windows, Linux, Mac), and also 
includes the capability of importing csv-files with predefined time series as input to slave 
variables. The simulator itself is a command-line tool that reads text files (project and 
data files) and writes results in csv-format text files as well, which makes it very suitable 
to be used in scripted environments (and optimization tools). In the upcoming releases the user 
interface will be extended to hold a graphical representation and include graphical routing,
and will exchange such systems/simulation scenarios via the SSP-standardized file formats.

