---
title: News from the FMI Project
author: Christian Bertsch, [MAP FMI](https://fmi-standard.org/)
category: association
---

{::options parse_block_html="true" /}

![FMI](FMI.png)

##### 16th International Modelica _and FMI_ Conference Sept 8-10 2025 in Lucerne, Switzerland

This conference was the first Modelica Association Conference that had the "FMI" also in its title - and it was a great success!
We had FMI- as well as industrial user track over the whole conference. This attracted about 40% more participants than at the last conference - especially from industry and attendants with main interest in FMI.
Key take-aways:

- FMI is used by almost everyone who visited the conference. Both in "standard use cases" - and in in many new cool applications and domains! 
- FMI 3.0 is getting the "new normal" - besides the widespread usage of FMI 2.0, in the majority of FMI-related presentation FMI 3.0 with its new features is used - and with growing tool support this accelerates fastly currently
- The Layered Standard concept hit a very important need to innovate fast without making the core standards too complicated.
- The FMI Layered Standard for Network Communication (FMI-LS-BUS) ist very fastly adopted (see below)
- At an FMI Advisory Committee Meeting the day after the conference with more than 50 participants, the FMI Project exchanged feedback, requirements and new ideas with many industry partners.

All FMI-related papers, tutorials and industrial user presentations on the [Literature page](https://fmi-standard.org/literature/) of the FMI website.

#### FMI Design meeting in Berlin 

![FMI Design Meeting Berling](FMI-Berlin.png 'FMI Dessign Meeting in Berlin, Dec 3/4 2025')

The FMI Project had a very productive FMI Design Meeting Berlin on Dec 3/4 2025. Good progress was made on

- extending the FMI Layered Standard for Network Communication (FMI-LS-BUS) from CAN (v1.0) to FlexRay, Ethernet and LIN, which will then cover the main automotive busses, and is open for extensions to other busses in many other fields such as automatisation, aerospace etc.
- the coming FMI Layered Standard for Structured Data (FMI-LS-STRUCT), for which we plan to enter beta stage soon.
- the coming FMI Layered Standard for reference (FMI-LS-REF), for which we will have an alpha version soon.
- enhancements of the FMI Standard w.r.t. to efficiency for large-scale, communication intensive simulations.

Many thanks to Dassault Systèmes and the local host Torsten Sommer for their hospitality! 

#### The FMI Layered Standard for Network Communication (FMI-LS-BUS) - growing tool support and extension for Flexray, Ethernet, LIN

![FMI-LS-BUS Roadmap](fmi-ls-bus-roadmap.svg 'FMI-LS-BUS Roadmap')

The year 2025 marks a significant advancement for the FMI Layered Standard for Network Communication (FMI-LS-BUS). With the release of version 1.0, a key milestone has been reached, laying the foundation for a standardized and flexible representation of networks in FMUs. In general the FMI-LS-BUS approach is suitable not only for the automotive industry but also for all domains, such as industrial automation, aerospace, and energy.

Version 1.0.0 offers, for the first time, full support for Physical Signal Abstraction and extends Network Abstraction to include the CAN, CAN FD, and CAN XL bus systems. This enables developers to model complex communication structures realistically and interoperably. This step is an important contribution to the unification of simulation standards and facilitates collaboration between different tools and platforms.

But that's not all: Throughout the year, further releases were published, continuously expanding the functionality of the FMI-LS-BUS. Version 1.1.0-Beta.2 introduced support for FlexRay, an essential bus for safety-critical applications. Shortly thereafter, version 1.2.0-Alpha.2 followed, which for the first time provides Ethernet support for the FMI-LS-BUS. In parallel, work on draft version 1.3.0 was completed, integrating the LIN bus – an important step for covering low-speed communication in distributed systems.

These developments clearly demonstrate that the FMI-LS-BUS is well on its way to establishing itself as a cross-industry standard. It offers a scalable solution for the growing demands on modeling communication systems in a wide variety of application areas.


#### Other Resources for FMI

* Visit the [FMI tools page](https://fmi-standard.org/tools) listing 260 tools supporting FMI!
* Join the [LinkedIn FMI community](https://www.linkedin.com/groups/7477473/) to get the latest news on FMI, FMI supporting tools and discussions within the user community.
* Report problems of the standard itself or suggestions for new features in form of issues or discussions on [fmi-standard.org](https://github.com/modelica/fmi-standard)
