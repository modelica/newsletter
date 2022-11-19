---
title: MultiflashMedia connector library
author: "Philip Jordan ([Dassault Systemes Deutschland GmbH](https://www.3ds.com/))"
category: "library"
---

The MultiflashMedia connector library was initially released with Dymola 2022x.
With Dymola 2023x, it has been updated to version 1.1.1. The library is an
interface to the external multi-component, multi-phase fluid property models and
solvers of the [Multiflash software package by
KBC](https://www.kbc.global/software/advanced-thermodynamics/).

![dassaultsystemes_multiflashmedia-connector.png](dassaultsystemes_multiflashmedia-connector.png 'The MultiflashMedia
Connector Library')

The library implements an object-oriented approach to the medium model. The
interface to Multiflash is provided in the form of the _Properties_-class. Its
instantiation in a Modelica component or system model is mirrored by a Modelica
External object. The external object handles the communication with the
Multiflash software. Among the supported flash calculation input
variable sets are _p,T,N-_, _p,h,N-_, _U,V,N-_, as well as fixed-phase _p,X,N-_
flashes. The library supports the thread-safe API features of the Multiflash
software and is suitable for simulation on multiple cores in Dymola.

The fluid configuration is file-based, using Multiflash Command File syntax and
file format. For Modelica models that require fluid properties for more than one
single mixture, the configuration of multiple mixtures with distinct components,
phases and models within a single command file is supported.