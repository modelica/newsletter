---
title: "Testing Library 1.8.0: Reimplemented functions tests"
author: "Marco Keßler ([Dassault Systèmes Austria GmbH](https://www.3ds.com/))"
category: "library"
---

Since the first release the Testing library supports unittests for Modelica functions.
However, this was always one of the weaker parts, as it required manual comparison of expected and actual values and setting the final test result.
Since Testing library 1.8.0 (shipped in spring with Dymola 2024x Refresh 1), test functions are much simpler to create, thanks to the new operator record `Testing.Functions.Check`.

The code snipped below shows how the algorithm section of a modern test function for the `Modelica.Math.isEqual` could look like:
```
  checks[1] := Check(
    expect = true,
    actual = isEqual(0.333, 1/3, eps=1e-3));

  checks[2] := Check(
    expect = false,
    actual = isEqual(0.333, 1/3, eps=1e-4));

  // if we expect true, we can also use the short version
  checks[3] := Check(isEqual(-0.333, -1/3, eps=1e-3));

  result := Check.summarize(checks);
```
You just have to pass the expected and the actual values to `Check`.
The `Check.summarize` functions computes the overall test result from our vector of checks and prints details when a check has failed. 

`Check` has constructors for `String`, `Integer`, `Boolean` and `Real` inputs, from scalar to 3D.
Comparing vectors of strings for example works similar as above:
```
checks[1] := Check(
  expect = {"angle", "force", "pressure"},
  actual = .Modelica.Utilities.Strings.sort({"force", "angle", "pressure"}));
```

More information about function tests can be found in the Testing library at `Testing.Functions.UsersGuide.`.
