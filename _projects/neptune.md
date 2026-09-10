---
layout: page
title: NEPTUNE
description: Performance portable plasma edge simulation for the exascale
img: assets/img/neptune.png
importance: 2
category: Plasma Physics
related_publications: true
---

[Project NEPTUNE](https://excalibur.ac.uk/projects/excalibur-fusion-use-case-project-neptune-neutrals-plasma-turbulence-numerics-for-the-exascale/) (NEutrals & Plasma TUrbulence Numerics for the Exascale) is the Fusion Use Case of the UKRI [ExCALIBUR](https://excalibur.ac.uk) programme. Led by the [UK Atomic Energy Authority](https://ccfe.ukaea.uk), it is building the simulation capability needed to design the exhaust system of a commercial tokamak, in direct support of the [STEP](https://step.ukaea.uk) programme.

The target is "the edge" -- the region where hot confined plasma meets cold neutral gas and the reactor wall. It is a classic multi-physics, multi-scale problem: fluid and kinetic models must be coupled across scales that differ by orders of magnitude, on machines whose architectures are still moving underneath us.

## My role

I lead the York contribution to **FM-WP4: Code Structure and Coordination**, funded across three consecutive UKAEA contracts, and am a co-investigator on **FM-WP2**, which developed the plasma fluid referent model through exploratory proxy applications.

The central question in WP4 is a pragmatic one: how do you write a simulation code today that will still run well on future compute hardware? Our work has surveyed the landscape of performance portable approaches for plasma edge simulation {% cite wright:2024:developing_pp_plasma %}, evaluated the maturity of SYCL compiler implementations as a portability vehicle {% cite shilpage:2023:sycl-compiler %}, and investigated domain-specific languages and code generation as a way of separating the physics from the hardware {% cite lantra:2024:op-pic %}.

That last strand produced **OP-PIC**, an unstructured-mesh particle-in-cell DSL that lets a single description of a fusion simulation be compiled to multiple parallel backends -- the alternative to maintaining a separate hand-tuned code per architecture.

## Collaboration

The project is a UK-wide effort. Our work has been carried out alongside the [York Plasma Institute](https://www.york.ac.uk/physics-engineering-technology/research/plasma/), the University of Warwick, and the wider NEPTUNE consortium {% cite threlfall:2023:neptune %}, and has been reported at ExCALIBUR programme-wide workshops {% cite wright:2022:neptune-poster %}.
