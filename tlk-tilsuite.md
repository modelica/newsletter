---
title: TLK TIL Suite - New version 3.7.0
author: "Matthias Kwak [TLK-Thermo GmbH](https://www.tlk-thermo.com/)"
category: "library"
---

{::options parse_block_html="true" /}

<div style="float: right">
![tlk-tilsuite logo](tlk-tilsuite-logo.png)
</div>

The TIL Suite is used to generate stationary and transient simulation results. It is based on technical experience with our test benches, and theoretical experience with services in the field of modelling and simulation. The next **version 3.7.0** will be available in **April 2019** and includes new and improved components and system models. Among other things, we would like to draw your attention to the following innovations:
- New VLEFluid-Volume model with fixed or variable volume including heat port.
- WallCell: Heat connections between wall cells with east-west orientation (along the channel) are now optional and disabled by default to reduce the sizes of the linear system of equations.
- Summaries: Property-calculations were changed, now using new TILMedia classes (object function based), which improve the compatibility to the Modelica specification.
- New VLEFluid-InlineBoundary model to set mass flow rate, temperature or heat flow rate at a certain position.
- New Watchdog model to terminate simulations after a defined time.
- VLEFluid-Pump2ndOrder: An improved energy balance for zero mass flow rate and the consideration of density by the affinity laws were added.


For further information see [www.tlk-thermo.com](https://www.tlk-thermo.com/index.php/en/software-products/til-suite), [download the TIL presentation](https://www.tlk-thermo.com/images/tlk/content/presentations/TIL_Suite_presentation.pdf) or contact us at [til@tlk-thermo.com](mailto:til@tlk-thermo.com).
