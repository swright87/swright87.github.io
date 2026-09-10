---
layout: page
title: FPGA for Scientific Computing
description: Reconfigurable architectures for computational science
img: assets/img/fpga.png
importance: 1
category: Performance Portability
related_publications: true
---

The computing power of HPC has been increasing at an exponential rate, recently passing the Exascale barrier. With this, the power consumption demands of HPC are ever-increasing, challenging the technical limits of what can be achieved. It is essential that solutions are found to achieving more performance within the same power envelope.

One possible solution to this is accelerating applications using dataflow architectures, an alternative accelerator hardware with potential to deliver better performance per Watt than a GPU. However, before dataflow architectures can see widespread use in HPC, there are challenges with portability and productivity that must be overcome.

This research is part of a three-year Ph. D. research project, aimed at identifying solutions to these challenges, both in the wider field of HPC and more specifically in the context of Unstructured Discrete Transport Algorithms, a class of wavefront algorithms related to particle transport.

This project is evaluating **SYCL** as a single-source, high-level entry point to FPGA compilation. We have been porting representative scientific kernels to Intel FPGAs and measuring what the abstraction actually costs.

## Results so far

We started with a structured heat diffusion mini-application to establish a baseline for the toolchain and the achievable performance {% cite storkey:2024:heat-fpga %}, then extended the work to unstructured stencil applications — a substantially harder case, where irregular access patterns undermine the pipelining the compiler depends on {% cite storkey:2025:fpga-sycl %}.
