---
title: FMI news
author: MAP FMI
category: association
---

{::options parse_block_html="true" /}

<div style="float: right">
![fmi-logo](fmi_logo_horizontal.svg)
</div>

#### FMI at the Modelica Conference - papers and tutorial available

#### FMI Compatibility Information on the FMI Tools list

The [FMI tools page](https://fmi-standard.org/tools/) now lists 192 tools supporting tools. 
And the four of them listed top and marked with the golden star now provides now contain a lin to "compatibility information" where they document how the tool vendors have tested their FMU import and export capabilities and standard compliance with other tools. 
Exporting tools also provide example FMUs, that can be tested by other importing tools.
This information is provided on an external webpage or repository provided by the tool vendors themselves.

![](FMI_tools_page.png)

(This replaces the [FMI Cross Check](https://github.com/modelica/fmi-cross-check), which has been archived)

#### FMI Design Meeting with guests after the Modelica Conference 2023 in Aachen, Germany

#### FMI Design Meeting in Nov 2023 in Sindelfingen, Stuttgart

FMI developers from Akkodis, AVL, Bosch, Dassault Systems, dSPACE, EKS-INTEC, ESI, ETAS, PMSF, Synopsys and Wolfram MathCore participated. Thanks to #Akkodis for the great hospitality!
We focused on layered standards to FMI 3.0
- [FMI-LS-XCP](https://github.com/modelica/fmi-ls-xcp) for XCP support (v1.0RC2 in preparation)
- [FMI-LS-BUS](https://github.com/modelica/fmi-ls-bus) for network communication (v1.0alpha in preparation)
- [FMI-LS-STRUCT](https://github.com/modelica/fmi-ls-struct) for maps and structuring of variables (concept work)
- and new ideas for layered standards reference source models, reference solutions, parameters sets.
Additionally we discussed possible efficiency optimizations for data transfer and access that can be addressed in FMI 3.1.

#### Call for Problems 

Currntly in the FMI project we start working on FMI 3.1, and would like the to ask the FMI user community to report their current pain points and ideas for future development.

Within the FMI project, we currenlty have the idea for FMI 3.1 to focus on efficiency topics: We have identified that for FMUs that handle a large amount of data communication compared to internal calculations, the current desig of FMI leads to overhead due to many copy operation of data. 
This could be either a very large amount of scalar variables, or array or binary variables. Severa solution approaches are in discussion, but currently the problem itself his not yet fully clear and has not yet been described in detail.
So if you face efficiency problems in the simulation of FMUs that can be traced back to communication

More generally, if you have problems w.r.t model exchange and co-simulation that cannot yet be solved well with FMI 3.0, please describe it and send it either in the form of an Github Isseu on https://github.com/modelica/fmi-standard/issues or send it via Email to contact@fmi-standard.org.
(We promise to reply, but not in which detail).

#### Resources and discussion forums for FMI related questions

* Join the LinkedIn FMI community: https://www.linkedin.com/groups/7477473/
* Ask technical questions and discuss topics on the usage of FMI on Stackoverflow tagged "FMI" https://stackoverflow.com/questions/tagged/fmi
* Report problems of the standard itself or suggestions for new features in form of issues on on fmi-standard.org https://github.com/modelica/fmi-standard/issues





