---
title: Simcenter Amesim 2210 FMI improvements
author: "Bruno Loyer ([Siemens Digital Industries Software](https://www.sw.siemens.com/ ))"
category: "vendor"
---

[Siemens Digital Industries Software](https://www.sw.siemens.com/ ) is proud to announce the recent release of [Simcenter Amesim 2210](https://blogs.sw.siemens.com/simcenter/whats-new-in-simcenter-system-simulation-2210/ ), as part of its system simulation solutions. Among the key features introduced in this release, we can highlight the FMI improvements below.

![](amesim_banner_2210.png)

## Leveraging Windows to Linux cross-compilation using FMI
With Simcenter Amesim 2210, you can create and share components with Linux users directly, from a 100% Windows ecosystem, without revealing any source code. To achieve this, neither Linux itself, nor any Linux virtual machine, nor even the Windows Subsystem from Linux (WSL) is required. Most of the time indeed, these “heavy” solutions are rejected by IT departments. To enable compiling for Linux, Simcenter Amesim 2210 simply needs to be installed on your Windows machine, which doesn't require any specific elevation of privilege. The secret behind this is a Windows to Linux cross-compiler that is now distributed as standard with Simcenter Amesim. Moreover, as FMI plays a central role in interoperability, this technical solution has been conveniently combined with FMI to offer the model deployment capabilities described hereafter.

### Direct export, from Windows, of FMUs usable under Linux 64-bit
A first clear benefit of the Windows to Linux cross-compiler now provided with Simcenter Amesim 2210 is the export of FMUs containing a Linux 64-bit binary now made possible under Windows in a few clicks. This allows creating highly portable cross-platform FMUs containing up to three different binaries (win32, win64 and linux64). This feature is designed to validate then deploy models to various Linux platforms, including Edge Computing, Cloud Computing, IIoT or HPC platforms.

![](amesim_multiplatform_fmu.png)

Thanks to this increased portability, it is for instance possible to use a Simcenter Amesim FMU exported under Windows:
* to define the boundary conditions of a [Simcenter STAR-CCM+](https://www.plm.automation.siemens.com/global/en/products/simcenter/STAR-CCM.html ) CFD model, or any model from an FMI compatible CFD tool, running on a Linux HPC cluster.
* as a high-fidelity “ego” vehicle model running in a [Simcenter Prescan](https://www.plm.automation.siemens.com/global/en/products/simcenter/prescan.html ) ADAS environment under Linux.

### Improved workflow for FMI based Linux 64-bit real-time targets
As a second benefit, from now on, the FMUs generated under Windows for any of the 64-bit Linux real-time targets officially supported by Simcenter Amesim are of type “binary”. In contrast to source-code FMUs, these binary FMUs are immediately usable; they no longer need to be compiled by the target’s toolchain. The FMI compatible real-time targets that benefit from this improved workflow are:
* [Concurrent SIMulation Workbench (SimWB)](https://concurrent-rt.com/products/software/simulation-workbench/ ) 64-bit
* ETAS LABCAR OPERATOR 64-bit
* [SIMATIC LiveTwin](https://www.youtube.com/watch?v=U7ay9eppRPw ) (Edge Computing Platform from Siemens)
* Simcenter Testlab RT (incubation product from Siemens) 
* Linux based target x64 (“generic” little endian target)

### Support of NI Linux Real Time OS (Intel x64) via FMI
The above-mentioned capability also enables the support of the recent [NI Linux Real Time OS](https://www.ni.com/en-us/shop/linux/introduction-to-ni-linux-real-time.html ), for which source-code FMUs are not suitable. These systems from NI progressively replace their older ones based on Phar Lap RT. They are typically used on NI [PXI](https://www.ni.com/en-us/shop/pxi.html ) or [CompactRIO](https://www.ni.com/en-us/shop/compactrio.html ) hardware. With Simcenter Amesim 2210, Windows users can now export their real-time capable models as binary FMUs for these systems directly. Under Linux, these FMUs are compiled using the local GCC.  

![](amesim_rt_fmu.png)

## Export of FMUs via a dedicated Python script
A new Python script allows exporting FMUs “offline” i.e., without having to open the Simcenter Amesim GUI. This script is functionally equivalent to the FMU Export Assistant GUI. It is thus capable to manage all kinds of FMUs that can be exported by Simcenter Amesim. Such an automated generation of executable digital twins can for instance be leveraged by [Simcenter Studio](https://www.plm.automation.siemens.com/global/en/products/simcenter/studio.html ) for reinforcement learning.    

![](amesim_FMU_scripting.png)

## Improved support of units and non-Latin titles
For an improved handling of exported FMUs, the units are now automatically declared and converted to the International System of Units. Optional conversion factor and offset are available for multiple/submultiple of (derived) SI units as well as for other custom units outside SI. On top of that, for better user experience and simplified collaborative work, UTF-8 titles of imported FMUs, containing non-Latin characters (e.g., Japanese or Chinese characters), are now fully supported by Simcenter Amesim.

## Towards FMI 3.0
In addition to the [“FMI terminals”](https://newsletter.modelica.org/2021-03/index#fmi-physical-terminals-between-simcenter-amesim-and-simcenter-flomaster ) feature, already supported by [Simcenter Amesim](https://www.plm.automation.siemens.com/global/fr/products/simcenter/simcenter-amesim.html ) and [Simcenter Flomaster](https://www.plm.automation.siemens.com/global/en/products/simcenter/flomaster.html ), [Siemens Digital Industries Software](https://www.sw.siemens.com/ ) plans to implement the support of FMI 3.0 in the forthcoming releases of its system simulation solutions. Stay tuned!

For more information on Simcenter Amesim, please visit our [website](https://www.plm.automation.siemens.com/global/en/products/simcenter/simcenter-amesim.html ).
