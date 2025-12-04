---
title: train_fmu_gym: Enabling FMU-based Deep Reinforcement Learning
author: "Johannes Ultsch [Department of Vehicle System Dynamics and Control, Deutsches Zentrum für Luft- und Raumfahrt (DLR)](https://www.dlr.de/)"
category: "library"
---

The [DLR Institute of Vehicle Concepts](https://www.dlr.de/en/fk), [Department of Vehicle System Dynamics and Control](https://vsdc.de) presents **train_fmu_gym**, a Python-based framework that utilizes the Functional Mock-up Interface (FMI) to leverage existing simulation models for deep reinforcement learning (DRL). The goal of train_fmu_gym is to enable users to easily set up and start DRL training, as well as evaluate trained agents based on system model FMUs, by providing a sophisticated command line interface (CLI). This allows existing Modelica and other FMI-based models to be reused directly for RL training without modifications to the underlying modeling workflow, bringing data-driven control methods closer to established engineering practice.

train_fmu_gym provides the following key features:
- Automated generation of DRL environments from FMI 2.0 and FMI 3.0 FMUs
- Flexible handling of different reward implementations and observation sets
- Definition, management, and use of simulation scenarios
- Integration of [Modelica Credibility](https://github.com/DLR-SR/Credibility) to define and handle uncertain scenarios
- Definition of evaluation metrics and execution of evaluation simulations to assess trained agents
- Support for setting up, training, and evaluating agents via more than 20 CLI functions
- Platform support for Linux and Windows

The toolchain is suitable for users who want a straightforward way to get started with RL on existing models, as well as for users who need deeper customization of environments, reward structures, and evaluation loops. It supports convenient iteration over environment versions and training configurations, enabling systematic experimentation until a satisfactory agent performance is achieved. The framework and example implementations are made openly available via the Helmholtz Cloud GitLab at: https://codebase.helmholtz.cloud/dlr-vsdc/train_fmu_gym

Further information about the framework is provided in the following contribution:
> J. Ultsch, K. Ahmic, and J. Brembeck,
> **"train_fmu_gym: A Functional Mock-up Unit-based Framework to Train Reinforcement Learning Agents for Multi-Physical Systems,"**
> *IEEE Access, 2025*,
> DOI: [10.1109/ACCESS.2025.3636787](https://doi.org/10.1109/ACCESS.2025.3636787)
