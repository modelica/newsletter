---
title: FMI news
author: Christian Berstch, [MAP FMI](https://fmi-standard.org/)
category: association
---

{::options parse_block_html="true" /}

![FMI](FMI.png)

#### News from the FMI Project

The FMI Project actively maintains the FMI 2.0.x and 3.0.x standards, and currently focusses on the development of Layered Standards to extend FMI for new application domains:

* [FMI-LS-XCP](https://github.com/modelica/fmi-ls-xcp) v1.0.0 released in Dec 2024: This layered standard defines support for [XCP](https://www.asam.net/standards/detail/mcd-1-xcp/) or “Universal Measurement and Calibration Protocol”, a network protocol defined by [ASAM](https://www.asam.net/). 
* [FMI-LS-BUS](https://github.com/modelica/fmi-ls-bus) v1.0.0 just released, see below. This layered standard defines how to realize the simulation of network communication with FMI 3.0 means.
* [FMI-LS-STRUCT](https://github.com/modelica/fmi-ls-struct) v1.0.0-alpha.1 prerelease: Based on FMI 3.0, this layered standard defines how variables (especially parameters) of an FMU can be structured and grouped in a more flexible way than with the “structured naming convention” of the FMI Standard. The first version of this layered standard is focused on the definition of sampled maps.
* [FMI-LS-REF](https://github.com/modelica/fmi-ls-ref) (in development). It will allow for the inclusion of related files into an FMU. This includes parameter sets, reference stimuli and results, which can be used in additional experiments, as well as other relevant files to the FMU, like the model sources, requirements, or specifications.

Additionally two new working groups for the improvement of efficiency of data communication between FMUs and for DAE support have been formed.

### FMI Design meeting in Berlin

We had a very productive FMI Design 

### The FMI Layered Standard for Network Communication - growing tool support and extension for Flexray, Ethernet, LIN

The year 2025 marks a significant advancement for the FMI Layered Standard for Network Communication (FMI-LS-BUS). With the release of version 1.0, a key milestone has been reached, laying the foundation for a standardized and flexible representation of networks in FMUs. In general the FMI-LS-BUS approach is suitable not only for the automotive industry but also for all domains, such as industrial automation, aerospace, and energy.

Version 1.0.0 offers, for the first time, full support for Physical Signal Abstraction and extends Network Abstraction to include the CAN, CAN FD, and CAN XL bus systems. This enables developers to model complex communication structures realistically and interoperably. This step is an important contribution to the unification of simulation standards and facilitates collaboration between different tools and platforms.

But that's not all: Throughout the year, further releases were published, continuously expanding the functionality of the FMI-LS-BUS. Version 1.1.0-Beta.2 introduced support for FlexRay, an essential bus for safety-critical applications. Shortly thereafter, version 1.2.0-Alpha.2 followed, which for the first time provides Ethernet support for the FMI-LS-BUS. In parallel, work on draft version 1.3.0 was completed, integrating the LIN bus – an important step for covering low-speed communication in distributed systems.

These developments clearly demonstrate that the FMI-LS-BUS is well on its way to establishing itself as a cross-industry standard. It offers a scalable solution for the growing demands on modeling communication systems in a wide variety of application areas.



##### 16th International Modelica _and FMI_ Conference Sept 8-10 2025 in Lucerne, Switzerland

Literature

Video recordings from the conference


##### FMI Beginners' Tutorial offered at the 16th International Modelica and FMI Conference

Video Recording#

![FMI-Beginners' Tutorial](FMI-Tutorial.jpg)


##### FMI Advisory Committee meeting after the 16th International Modelica and FMI Conference, Sept 11 2025 in Lucerne

Report 

##### Other Resources and Discussion Forums for FMI-related Questions

* Visit the [FMI tools page](https://fmi-standard.org/tools) listing 250 tools supporting FMI!
* Join the [LinkedIn FMI community](https://www.linkedin.com/groups/7477473/) to get the latest news on FMI, FMI supporting tools and discussions within the user community.
* Ask technical questions and discuss topics on the usage of FMI on [StackOverflow tagged "FMI"](https://stackoverflow.com/questions/tagged/fmi).
* Report problems of the standard itself or suggestions for new features in form of issues or discussions on [fmi-standard.org](https://github.com/modelica/fmi-standard)
