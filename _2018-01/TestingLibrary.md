---
title: Testing Library 1.0 - Create and run regression tests 
author: "Imke Krüger ([Dassault Systemes](https://www.3ds.com/))"
category: "library"
---

The Testing Library is a Modelica Library available to all Dymola users. 
With this library it is possible to build test cases, create reference results and run the tests –
all within Dymola. It allows detecting unwanted side effects on model changes in an early
stage by running regular tests. The library contains multiple blocks for the continuous
comparison of signals to reference values and trajectories. Existing examples and test
models can easily be converted to a test case by providing a reference and connecting the
signals of interest to one of the various comparison blocks.

Test models can be simulated as any other model. At the end of the simulation the
message window shows the test result for every check block in the model.
This allows the developer to check regularly during the development if the tests class behaves as expected.

