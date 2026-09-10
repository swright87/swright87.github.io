---
layout: page
title: P3 Analysis Library
description: Quantifying performance, portability, and productivity trade-offs
img: assets/img/p3.png
importance: 2
category: Performance Portability
related_publications: true
---

When considering the development of a new simulation application, we are typically interested in maximising **performance**, **portability**, and **productivity**. In terms of _performance_ we are usually concerned with metrics that directly measure or affect the "time-to-science", while for _portability_ we are usually concerned with an application's ability to run correctly on different HPC systems and architectures. _Productivity_, on the other hand, is usually a measure of the time and expertise required to develop and maintain the application.

The [**P3 Analysis Library**](https://p3hpc.org/p3-analysis-library/) is an open-source Python toolkit for calculating, plotting, and reasoning about the performance, portability, and productivity of scientific applications. It standardises the collection of performance data across platforms and computes the metrics the community has settled on -- **performance portability** and **code divergence** -- alongside visualisations such as cascade plots and navigation charts that expose where an application's efficiency is actually going.

## The P3 Explorer

Metrics are only useful if there is something to compare against. The [**P3 Explorer**](https://p3-explorer.github.io) {% cite smith:2025:p3-explorer-paper smith:2024:p3-explorer-poster %} is an open database of performance, portability, and productivity results. It collects published P3 data into one queryable place so that claims about portability can be checked rather than taken on trust.
