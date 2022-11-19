---
title: Announcing Dymola 2023x
author: "Dag Brück ([Dassault Systemes](http://www.3ds.com/dymola))"
category: "vendor"
---

We are pleased to announce that Dymola 2023x will be available in November 25, 2022. 
![Dymola 2023x](Dymola-2023x.png)

#### Model editing

It is now possible to view (read-only) libraries and your own files in separate browsers. This makes the separation clear, and you can arrange the browsers around your Dymola window to fit your workflow. The traditional view is the initial default.

The handling of external resources associated with a model, such as, images in the documentation or data tables on file, has been improved. This means that when moving or copying a model the resources are copied to the same relative location.

#### Simulation

Commands that perform multiple simulation can change any parameter, lifting the earlier restriction that evaluated parameters cannot be changed. However, changing a structural parameter will of course add the overhead of translating the model.

#### Model import and export

Dymola 2023x is the first release to support the much-awaited FMI 3.0 file format that is expected to gain wide acceptance. New features of FMI 3 (arrays, ports and terminals, early return to handle events) will be supported in the near future.

SSP import supports Simulation Resource Meta Data (SRMD) stored in the SSP file. The meta data has been proposed to facilitate a credible simulation process with an adaptable format.
