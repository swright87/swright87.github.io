---
layout: page
title: EPOC++
description: Re-engineering a production laser-plasma PIC code for exascale
img: assets/img/epoc.png
importance: 1
category: Plasma Physics
related_publications: true
---

**EPOCH** is a relativistic particle-in-cell code used across the international laser-plasma community to simulate high-intensity laser interactions with matter. It has been in production for well over a decade and carries a substantial user base. Unfortunately, the Fortran codebase predates mass adoption of GPUs.

[**EPOCpp**](https://warwick-plasma.github.io/EPOCpp/) is the answer to that: a ground-up re-engineering of EPOCH in modern C++, designed so that the physics is expressed once and the performance-critical loops can be retargeted at whatever accelerator the next machine ships with.

## My role

I am the Principal Investigator at York for **EPOC++: A Future-proofed Kinetic Simulation Code for Plasma Physics at Exascale**, funded by EPSRC ([EP/W029111/1](https://gow.epsrc.ukri.org/NGBOViewGrant.aspx?GrantRef=EP/W029111/1).

The work is a collaboration with the [Centre for Fusion, Space and Astrophysics](https://warwick.ac.uk/fac/sci/physics/research/cfsa/) at Warwick and the [York Plasma Institute](https://www.york.ac.uk/physics-engineering-technology/research/plasma/). Progress has been reported at the High Power Laser meetings {% cite bennett:2024:epoc-poster goffrey:2025:epoch-poster %}.
