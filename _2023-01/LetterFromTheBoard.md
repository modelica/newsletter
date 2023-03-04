---
title: Letter from the Board
author: "Martin Otter ([Modelica Association](https://www.modelica.org/))"
category: "letter"
---

Dear Modelica, FMI, SSP, DCP, eFMI interested,

The **[International Modelica Conference 2023](https://2023.international.conference.modelica.org/)** will take place **Mo. Oct. 9 - Wed. Oct. 11, 2023, in Aachen, Germany**, as a **face-to-face conference**. Deadline for scientific paper and industrial user presentation submissions is **May 26, 2023**. For more details, see [article](#Modelica-Conference2023-Call-for-Papers).\
If you are interested to organize the next International Modelica Conference in 2025, please contact me.

**[Version 3.6 of the Modelica Language](https://specification.modelica.org/master/)** is finalized and will be soon formally released. It contains new features such as *multilingual support of Modelica* or *inheriting a model and removing some parts*. For more details, see [article](#Modelica-3.6-announcement).

The **[FMI 3.0 implementors guide](https://modelica.github.io/fmi-guides/main/fmi-guide/)** has been released. It gives non-normative recommendations for providing FMI 3.0 support in tools, but also using it. As an example, have a look at [section 9.1.2](https://modelica.github.io/fmi-guides/main/fmi-guide/#adjointDerivatives) that shows how to efficiently compute gradients of FMI 3.0 models for artificial intelligence (AI) frameworks via *adjoint derivatives*. Teasers for some FMI 3.0 features are available as [Jupyter notebooks with Python code](https://github.com/t-sommer/fmi3-features). You can [run these notebooks in your browser](https://mybinder.org/v2/gh/t-sommer/fmi3-features/HEAD) without any installation. We see more and more tools that support FMI 3.0. For the actual status, see [FMI tools](https://fmi-standard.org/tools/) and select *FMI Version 3.0*.

The MAP (Modelica Association Project) FMI currently works mainly on **layered standards** for certain extensions of FMI 3.0, e.g., for simulation of network communication. Also, [eFMI](https://efmi-standard.org/) can be seen as an extremly powerful layered standard extension of FMI. Layered standards are a concept first introduced in the SSP standard, and then adopted to FMI. See [FMI 3.0, section 2.6]( https://fmi-standard.org/docs/3.0/#VersioningLayered) for more information. It allows to perform open source and commercial extensions of the FMI standard in a backwards compatible way, in particular also by third parties that have no relation to MAP FMI.

<img align="right" src="https://github.com/modelica/newsletter/blob/main/_2022-03/ma-t-shirt.png">

The MA (Modelica Association) board has finally decided to base the MA web pages technically on the static site generator [Hugo](https://gohugo.io/) using the [fmi-standard.org](https://fmi-standard.org/) web page as a template. Hugo has the advantage that it is simple to use (just download and run the executable for your platform; provide content especially with markdown files), has a modern layout and is actively maintained. For more info, see the [sources of the fmi-standard.org website](https://github.com/modelica/fmi-standard.org) and the [ma-hugo-theme](https://github.com/modelica/ma-hugo-theme). In the near future, all other MAPs and the MA entry web page will be based on Hugo.

Recall that Modelica Association has now a [Spreadshirt Shop](https://ma-merch.myspreadshop.de/) where you find T-Shirts, hoodies, coffee cups and stickers with various logos from the Modelica Association and its standards.

If you have interesting news for the Modelica, FMI, SSP, DCP, eFMI communities, please follow the [submission guidelines](https://newsletter.modelica.org/submission-guidelines.html). The deadline for articles for the next newsletter is Friday, July 7, 2023.

Martin Otter on March 3, 2023

Chairperson of the Modelica Association
