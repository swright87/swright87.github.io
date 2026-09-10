---
layout: page
title: POSE
description: The Power-Optimised Software Envelope for energy-aware optimisation
img: assets/img/pose.png
importance: 1
category: Energy-Aware Computing
related_publications: true
---

Until recently Koomey's law -- which posits that the electrical efficiency of computation has doubled roughly every year and a half -- has meant that the exponential growth in performance predicted by Moore's law has been achieved without a corresponding increase in power consumption. However, there is substantial evidence that Koomey's law is slowing, meaning that power is fast becoming a primary constraint on the size and performance of new HPC systems. As awareness of energy use and wastage grows among both users and system administrators, it becomes increasingly critical to prioritise energy efficiency in the development of scientific computing applications for HPC systems.

The **Power-Optimised Software Envelope** (POSE) is a modelling framework that allows a user to analyse the trade-off between application run time and power consumption, showing the scope that may be available for _energy-aware optimisation_. Given a measurement of an application's current behaviour, POSE bounds the energy savings available from further optimisation, so a developer can decide whether the effort is justified — and which of speed or power is the more promising direction {% cite roberts:2019:pose-taco roberts:2015:pose %}.

The framework grew out of work on multi-objective metrics for energy-aware software optimisation {% cite roberts:2017:metrics %}, which addressed the prior question of what "better" even means when two objectives are in tension.

## Current work

POSE is being extended to account for the memory hierarchy. The original model treats the application as a single aggregate; **cache-aware POSE** recognises that where data sits dominates both the time and the energy of a computation, and that an energy bound which ignores this leaves a great deal on the table {% cite pasupuleti:2026:ca-pose %}.

## Code

The model, benchmarks, and data collection scripts are available from the [POSE organisation on GitHub](https://github.com/pose-model), including the `Pmin` benchmarks that establish the minimum power draw of a system still doing useful work, a spreadsheet implementation of the model, and the cache-aware extension.
