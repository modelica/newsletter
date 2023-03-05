title: Claytex technical blog
author: "Mahdieh Mehrabi ([Claytex](https://www.claytex.com/))"
category: "education"
---

![Claytex logo]( https://www.claytex.com/wp-content/uploads/2022/05/Claytex-TECHNIA-COMPANY-RGB-217-90.png "Claytex logo")

Claytex publishes a [technical blog](https://www.linkedin.com/showcase/our-technical-blog/) covering all things Modelica and Dymola.

#### Documentation in your Dymola Models

I spend a lot of time looking at Dymola models created by others, and a big factor in a model’s user friendliness is the quality of the documentation included. So, in this blog post, I’m going to take a look at the documentation options available in Dymola.

![Documentation Image1]( https://www.claytex.com/wp-content/uploads/2023/02/Documentation-Image-1_Modelica-NL.png "Documentation Image1")

Read the complete article [here]( https://www.claytex.com/blog/methods/documentation-in-your-dymola-models/)

#### Improve performance by using different compilers in Dymola

Sometimes using a different C compiler can result in a model simulating faster. In this post we look at how the different Windows compilers, Visual Studio, Visual Studio with Clang, MinGW and MinGW with Clang can be used to compile a Dymola model and potentially create executables that simulate the models faster.

![Improve performance Image2]( https://www.claytex.com/wp-content/uploads/2023/02/Improve-performance-Image-2_Modelica-NL.png "Improve performance Image2")

Read the complete article [here]( https://www.claytex.com/tech-blog/improve-performance-by-using-different-compilers-in-dymola/)

#### What can you get out of a detailed simulation? Taking a look at a Fuel Cell electric bus model

Last year as part of the 2022.1 release of the VehicleDemos library, Claytex added a Hydrogen Fuel Cell Electric (FCEV) bus model. Created out of the existing EV bus example, it showcased integrating models from the Hydrogen Library with VeSyMA vehicle models. Ambitiously, a high level of detail was included. Physical air and hydrogen supply models were built, coupling with a fuel cell stack model where current production was dependent upon the pressure and temperature of the reactants. 

![Fuel Cell Electric Bus Image3]( https://www.claytex.com/wp-content/uploads/2023/02/Fuel-Cell-Electric-Bus-Image-3_Modelica-NL.png "Fuel Cell Electric Bus Image3")

Read the complete article [here]( https://www.claytex.com/tech-blog/what-can-you-get-out-of-a-detailed-simulation-taking-a-look-at-a-fuel-cell-electric-bus-model/)

#### Simulating KnC Rigs

The Suspensions library is full of experiments that test the full vehicle dynamics. However, it can be very difficult to validate models using full vehicle experiments, such as the common Kinematic and Compliance (KnC) test. This kind of test, as the name suggests, details the suspension kinematics (force and movement as the result of regular suspension operation) and the compliance (amount of force and movement in directions that aren’t bump or steering) of a vehicle.
These tests are conducted on KnC rigs, which are large experiment platforms with actuators and measuring equipment, normally designed to test full vehicles. How this is done is dependent on the tests carried out, but in its simplest form it consists of 4 pads that support the vehicle, which can be moved up and down to simulate road input. This tests suspension reaction to known inputs, such as sinusoidal sweeps or measured road inputs.

![Simulation KnC Rigs Image4]( https://www.claytex.com/wp-content/uploads/2023/02/Simulation-KnC-Rigs-Image-4_Modelica-NL.png "Simulation KnC Rigs Image4")

Read the complete article [here]( https://www.claytex.com/tech-blog/simulating-knc-rigs/)
