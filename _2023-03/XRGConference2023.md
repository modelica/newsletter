---
title: XRG Product News and Contributions to the International Modelica Conference 2023
author: "Stefan Wischhusen [XRG Simulation GmbH](https://www.xrg-simulation.de/en)"
category: "vendor"
---

### Our Product NEWS
#### XRG HumanComfort und FluidDynamics Library

XRG offers two unique Modelica libraries that enable Navier-Stokes-based CFD coarse grid simulations in Dymola and Modelica. Profit from seamless coupling with system models and less computational effort for transient simulations.

Pre-processing and post-processing is provided by our **Score lite** Application which is a complementary feature of [HumanComfort](https://www.xrg-simulation.de/en/products/xrg-library/humancomfort) and [FluidDynamics Library](https://www.xrg-simulation.de/index.php/en/products/xrg-library/fluiddynamics). If you already hold licenses of one or both libraries and do not have Score yet: Get in touch with us and [request](mailto:humancomfort@xrg-simulation.de?subject=Request%20for%20Score%20lite) your **free** license of Score lite today.

 ![XRG Coarse Grid CFD Tool-Chain](https://www.xrg-simulation.de/sites/default/files/inline-images/ScoreLite900.png 'XRG Coarse Grid Tool-Chain using FREE Score lite')

#### XRG HVAC Library

The newest version 3.0.0 of our [HVAC Library](https://www.xrg-simulation.de/en/products/xrg-library/xrg-hvac-library), offering the fastest HVAC simulations on the market, is now available for 

 - Dymola (Dassault Systèmes)
 - OpenModelica
 - Impact (Modelon)
 
 ![HVAC Library 3.0.0](HVAC_3.jpg 'HVAC Library 3.0.0 offers multi-tool support')

The HVAC Library includes components to model conventional energy systems with gas or oil boilers, as well as sustainable, CO2-neutral systems with heat pumps, solar thermal collectors, photovoltaics and storage units. 
By using a pressure-free modelling approach, simulation results can be delivered very fast, even for complex systems. This makes the models ideal for annual simulations and automated optimization techniques.

The new version 3.1.0 of the HVAC Library got a comprehensive update and improvement of many component models which will be presented in the XRG vendor session on Mon., 9th (see above).

#### XRG Score Application

[XRG Score](https://www.xrg-simulation.de/en/products/applications/score) executes parallel Dymola or FMU simulations, imports **large** Dymola or OpenModelica result files and lets you filter and interpolate them. Our Score Application allows you to define and save all your simulation settings, model parameters and any results you require in a workbook and directly share them with others. You can run, import and report on any number of simulations over one of these workbooks. You can automatically transfer the results in Excel spreadsheet templates along with integrated charts and formulas.

 ![XRG Score Add-in](https://www.xrg-simulation.de/sites/default/files/2018-05/XRG-Grafik-Score-Kompatibilitaet-e-20180514.png 'XRG Score interaction with Excel and Dymola or FMU')

More technical features of Score:
  - **Multi-Threading** (parameter sweeps on multiple CPU cores) of Dymola or FMU simulations
  - **Automatized** simulation process
  - Import, filtering and interpolation of complex result files (Dymola, FMU and OM) in Excel
  - **Easy exchange** of Excel workbooks
  - Template reports
  - Broad support of MS Office versions through COM add-in
  
The new version 1.9 incorporates some interesting features about post-processing of HumanComfort and FluidDynamics CFD results and more. Please attend the XRG vendor session on Mon., 9th (see above).

#### ClaRaPlus Library

 ![ClarRa 1.7.1](ClaRaPlusInfoHeader171.png 'Advanced power plant simulation')

Well established [ClaRaPlus Modelica library](https://www.claralib.com/index.php?lang=en) provides its users with the capability to proficiently tackle tasks in the disciplines of thermal hydraulics, instrumentation and control pertaining to power plants and other kind of energy systems. Based on the needs of steadily growing community of ClaRaPlus users community, it has broadened its scope over the years of its development, transcending the original focus on conventional power plants to encompass renewable power plants, waste heat utilization, general process plants, refrigeration cycles, heat pumps and beyond.

The recent version 1.7.1 of ClaRaPlus brings an exciting addition to the already impressive suite of features - support for the utilization of various artificial intelligence models in Modelica simulation tools.

Some of the key features are:
- Detailed models of turbo machinery, 4Q pump/compressor, piping, valves, heat exchangers, furnace, fluidized bed, drum, coal mill
- Demonstrators for **Coal/Combined/ORC power plant**
- **DCS package** – ready-to-use state of the art control blocks and controller examples
- **Grid package** – enables investigations of interactions with the electrical grid
- Flexible and user-friendly with efficient means for simplified **steady state analysis** (via StaticCycles models) for the calculation of consistent initial values for states to smooth the initialisation of complex thermodynamic cycles
- Well defined model design principles including level of detail, level of insight, naming conventions, limited inheritance depth, comprehensive documentation, and more
- **Extensive Media Library** – including ORC Media and steel data base
- **Support for AI** (see SMARTIInt Library)
- Validated against literature and measurement data

#### XRG's open-source products

 We have moved all our current open-source products to [Github](https://github.com/xrg-simulation). **You are welcome to start collaborating today!**

  ![Our Open-Source Products on GITHUB](XRGGithub.jpg 'Our Open-Source Products on GITHUB')

**SMARTIInt**<br>
SMARTIInt provides a user-friendly interface between Modelica and data-based AI models. With its first release the SMARTIInt Modelica library provides integration of TensorFlow neural networks (feed forward and recurrent) as Modelica functions. SMARTIInt can be found on [Github](https://github.com/xrg-simulation/SMArtIInt). 
We intend to support further data formats and network structures in the future. Community feedback and help are highly welcome!

**ClaRaDelay**<br>
Unlike the Modelica delay operator, ClaRaDelay also supports vectorized delay time inputs. This is especially useful when it comes to convolution integrals or other control applications. See [Github](https://github.com/xrg-simulation/ClaRaDelay) for details.

**ClaRa Library goes GITHUB**<br>
The open-source library ClaRa enables detailed analysis of power plant processes in Modelica and now broadens its scope towards renewable energies. Its official releases are now also available from [Github](https://github.com/xrg-simulation/ClaRa-official). With the newly established [ClaRa Open Development Repository](https://github.com/xrg-simulation/ClaRa-openDevelopment) we encourage the community not only to give feedback but also to participate in ClaRa's development by contributing models. Don't miss our presentation **"Status of the ClaRa Library: Detailed Transient Simulation of Complex Energy Systems"**([Link to session](https://www.conftool.com/modelica2023/index.php?page=browseSessions&form_session=45)) at the 15th Modelica conference!  



