---
title: "FMI-based Digital Twins in European Projects on Railways"
author: "Andreas Heckmann (DLR), Alex Meierhofer (VIF), Blas Blanco Mula (CAF)"
category: "association"
---

![MAP eFMI®](MAP-eFMI.png "MAP eFMI®")

#### _eFMI® Standard 1.0.0 Beta 1_ released

The next [candidate-draft](https://www.efmi-standard.org/standard/#release-cycle-and-versioning), the _eFMI® Standard 1.0.0 Beta 1_, for the first official release of the _eFMI® Standard_ has been released! You can find it on the official eFMI® website, https://www.efmi-standard.org/.

This is the first Beta release since the last candidate-draft, the Alpha 4. We are therefore now in beta phase, with each beta finalizing one model representation chapter.

This release focuses on the Behavioral Model representation, whose specification has been finalized and significantly extended and improved to achieve semantic completeness. Among many features, eFMI® Behavioral Models support:

 - testing of any other eFMI® model representation like Algorithm, Production or Binary Code
 - equidistant and variable time grid scenarios, the former with well-defined acceptable time-deviation and the latter with well-defined interpolation semantic
 - tolerances configurations defining the absolute and relative error tolerances of variables for various floating-point precisions
 - mapping configurations defining how to map variables of any dimensionality (scalar, vector, matrix, or higher dimensionality) to reference trajectories stored in CSV files
 - proper handling of time grids w.r.t. actual (i.e., used to conduct a test) and presupposed (i.e., assumed by the test provider) sampling times
 - proper handling of units of reference trajectories and tolerances
 - testing of error signals, including test scenarios with expected errors
 - test scenarios with runtime recalibration of tunable parameters
 - clear requirements on test environments and definition of how to conduct a test

Besides the _"Behavioral Model representation"_ Chapter, Beta 1 also finalizes the PDF layout and support chapters, like:

 - footer with standard version, current page number and total, licensing and website link
 - use of single open source font family
 - blank pages for correct printing
 - _"Legal information"_ Chapter, now with colophon stating the licenses of used open source fonts, trademarks and disclaimer
 - the title page, now with eFMI® logo.

There are only minor improvements in the other chapters; they will be focused on and finalized in individual future Beta candidate-drafts. The plan for Beta 2 is to wrap up the current preamble with _"Abstract"_, _"Overview"_ and _"Introduction"_ Chapters into a single _"Overview"_ Chapter, wrap up and finalize Chapter 1, _"General Concepts"_, and Chapter 2, _"eFMU container architecture"_, into a single _"Common concepts"_ chapter, and finalize Chapter 3.1, the _"Algorithm Code manifest"_.

Testing -- and how to define tests, store references, integrate the tooling subject to testing, and make sure different test environments agree on the test results for a certain tooling -- is certainly a hot topic for any Modelica Association standard and project. We sincerely hope that the _eFMI® Standard 1.0.0 Beta 1_ provides an excellent starting point for discussion and insights on the challenges of achieving well-defined semantics and completeness, even if "just" for something as "simple" as testing sampled data systems.

If you have any general questions, feedback or improvement proposals for the _eFMI® Standard_, please follow the [reporting specification issues and new feature requests guidelines on our website](https://www.efmi-standard.org/standard/#reporting-specification-issues-and-new-feature-requests) or contact us on our _public_ mailing list, [`efmi-info@googlegroups.com`](https://groups.google.com/g/efmi-info) (no Google account required).

**Your feedback is very welcome!**
