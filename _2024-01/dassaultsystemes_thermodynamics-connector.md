---
title: Thermodynamics Connector library
author: "Philip Jordan ([Dassault Systemes Deutschland GmbH](https://www.3ds.com/))"
category: "library"
---

The Multiflash Media Connector library has been renamed to Thermodynamics
Connector library with the upcoming Dymola 2024x Refresh 1 release. The reason
for the change in name is the expanded functionality beyond the existing
interface to Multiflash external equilibrium solvers and fluid property data.

In addition to the Multiflash interface, the Thermodynamics Connector library
v1.2.0 now provides an interface to CAPE-OPEN compatible property packages. The
new interface supports the integration of external multi-phase, multi-component
phase equilibrium calculations from CAPE-OPEN supporting software into Modelica models.

The CAPE-OPEN standard enables CAPE (Computer-Aided Process Engineering)
applications to interoperate. CAPE-OPEN is developed and maintained by the
CO-LaN organization ([CAPE-OPEN Laboratories Network,
www.colan.org](https://www.colan.org)). Dymola, with the Thermodynamics
Connector library, is the first PME (Process Modelling Environment) to implement
CAPE-OPEN’s COBIA middleware. COBIA is the platform independent replacement for
the legacy, COM-based CAPE-OPEN architecture.
