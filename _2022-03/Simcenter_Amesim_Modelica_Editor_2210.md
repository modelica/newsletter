---
title:  Simcenter Amesim 2210
author: "Karim Besbes ([Siemens Digital Industries Software](https://www.sw.siemens.com/)"
category: "vendor"
---

[Siemens Digital Industries Software](https://www.sw.siemens.com/ ) is proud to announce the recent release of [Simcenter Amesim 2210](https://www.plm.automation.siemens.com/global/en/products/simcenter/simcenter-amesim.html ), as part of its [system simulation solutions](https://www.youtube.com/watch?v=PNvEug8pcDM ). Among the key features introduced in this release, we can highlight the Modelica Editor related improvements and the FMI improvements below.

**Simcenter Amesim** offers a full-featured editor for the Modelica language that enables using and maintaining  Modelica legacy code and building your own Modelica-based models. Thus this complete integrated development application, the **Modelica Editor**, creates bridges between the **acausal** world of Modelica and the **causal** environment of Simcenter Amesim. 

![](ModelicaEditorBanner.png)

#### Automatic generation of iteration variables and their guess values

As of Simcenter Amesim 2210, the **Modelica editor** provides a new toolbar button allowing to automatically generate the iteration variables of a selected model during compilation. As shown in the following figure, the iteration variables are defined in a <i> record </i> and automatically added to the model code to be reused directly from the Simcenter Amesim parameters panel.

![](Editor2210.png)

#### Modelica Editor's new capabilities

The latest version of Modelica Editor contains other new features, the most important of which are:
* A new option now available in the Modelica preferences, enabling **parameter evaluation** as a means to reduce significantly the simulation time.
* A dedicated widget for your already-compiled models that are now seperated from your library tree, as shown in the figure above. 
* An easy update of your Modelica models directly in the Modelica Editor and a faster troubleshooting.
* An active tab now linked to its Modelica class highlighted in the library tree.
* Non-Latin (UTF-8) characters, like Asian characters, are now fully supported in Modelica descriptions and reflected without any changes once in Simcenter Amesim.


#### FMI improvements

- **Leveraging Windows to Linux cross-compilation using FMI** With Simcenter Amesim 2210, you can create and share components with Linux users directly, from a 100% Windows ecosystem, without revealing any source code. [More details](amesim_details.html)
  - Direct export, from Windows, of FMUs usable under Linux 64-bit
  - Improved workflow for FMI based Linux 64-bit real-time targets
  - Support of NI Linux Real Time OS (Intel x64) via FMI
- **Export of FMUs via a dedicated Python script** A new Python script allows exporting FMUs “offline” i.e., without having to open the Simcenter Amesim GUI. [More details](amesim_details.html)
- **Improved support of units and non-Latin titles** For an improved handling of exported FMUs, the units are now automatically declared and converted to the International System of Units. [More details](amesim_details.html)
- **Towards FMI 3.0**
In addition to the [“FMI terminals”](https://newsletter.modelica.org/2021-03/index#fmi-physical-terminals-between-simcenter-amesim-and-simcenter-flomaster ) feature, already supported by [Simcenter Amesim](https://www.plm.automation.siemens.com/global/fr/products/simcenter/simcenter-amesim.html ) and [Simcenter Flomaster](https://www.plm.automation.siemens.com/global/en/products/simcenter/flomaster.html ), [Siemens Digital Industries Software](https://www.sw.siemens.com/ ) plans to implement the support of FMI 3.0 in the forthcoming releases of its system simulation solutions. Stay tuned!

For more information on Simcenter Amesim improvements, please check this [blog post](https://blogs.sw.siemens.com/simcenter/whats-new-in-simcenter-system-simulation-2210/ ). For more information on Simcenter Amesim in general, please visit our [website](https://www.plm.automation.siemens.com/global/fr/products/simcenter/simcenter-amesim.html).
