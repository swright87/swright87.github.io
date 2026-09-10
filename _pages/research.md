---
layout: page
title: Research
permalink: /research/
description:
nav: true
nav_order: 3
display_categories: [work]
horizontal: false
---

I've been working in the High Performance Computing (HPC) research field since 2010, and in this time I have collaborated widely with other universities, UK and US national laboratories, and industry.
Much of my recent work has been focussed on the performance, portability and programmability of applications of interest to the Plasma Physics community.
These projects have been funded under the ExCALIBUR Fusion Use Case ([Project NEPTUNE](https://excalibur.ac.uk/projects/excalibur-fusion-use-case-project-neptune-neutrals-plasma-turbulence-numerics-for-the-exascale/)) and by EPSRC ([EP/W029111/1](https://gow.epsrc.ukri.org/NGBOViewGrant.aspx?GrantRef=EP/W029111/1)).

Broadly speaking, my research interests fall into three categories:

#### Performance Analysis and Optimisation

- Design and development of low-overhead performance analysis tools
- Novel performance models and modelling techniques
- Evaluation of new programming models and novel hardware
- Quantifying performance portability

#### Parallel File Systems and I/O

- Analysis of parallel file systems and bottlenecks
- Development of portable file structures and data structures
- Replication of sensitive I/O patterns in open environments
- Optimisation of parallel file systems on many-user systems

#### Energy-aware Computation

- Multi-objective optimisation metrics for energy-aware computing
- Heuristic performance models for energy/power
- Reconfigurable computing for computational science

A summary of the projects these interests have turned into is on the [projects page]({{ '/projects/' | relative_url }}).

## Research Group

### Current Ph.D. Students

- [Matthew Smith](https://www.cs.york.ac.uk/people/?group=Research%20Students&username=masmith) (started 2025) — performance, portability, and productivity of scientific computing applications; the [P3 Explorer]({{ '/projects/p3-analysis-library.html' | relative_url }}).
- [Suryachandra Pasupuleti](https://www.cs.york.ac.uk/people/?group=Research%20Students&username=spasup) (started 2024) — energy-aware MLSys and SysML and the [Power-Optimised Software Envelope]({{ '/projects/pose.html' | relative_url }}).
- [Zadok Storkey](https://www.cs.york.ac.uk/people/?group=Research%20Students&username=zabelg) (started 2023) — [SYCL on FPGAs]({{ '/projects/fpga.html' | relative_url }}) for structured and unstructured scientific applications.
- [Serdar Bulut](https://www.cs.york.ac.uk/people/?group=Research%20Students&username=sbulut) (started 2022, part-time) — optimising checkpoint write performance to parallel file systems using LSM-trees.

### Postdoctoral and Visiting Researchers

- Dr. Andrew Naden — Postdoctoral Research Assistant, 2023–2025.
- [Giulio Malenza](https://alpha.di.unito.it/giulio-malenza/) — Visiting Student, University of Turin, 2025.

## Ph.D. Opportunities

HPC has a vibrant research community, and if you'd like to be part of that community, there are Ph.D. opportunities available. Please get in touch to discuss potential projects.

{% comment %}
<!-- pages/projects.md -->
<div class="projects">
{%- if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized projects -->
  {%- for category in page.display_categories %}
  <h2 class="category">{{ category }}</h2>
  {%- assign categorized_projects = site.projects | where: "category", category -%}
  {%- assign sorted_projects = categorized_projects | sort: "importance" %}
  <!-- Generate cards for each project -->
  {% if page.horizontal -%}
  <div class="container">
    <div class="row row-cols-2">
    {%- for project in sorted_projects -%}
      {% include projects_horizontal.html %}
    {%- endfor %}
    </div>
  </div>
  {%- else -%}
  <div class="grid">
    {%- for project in sorted_projects -%}
      {% include projects.html %}
    {%- endfor %}
  </div>
  {%- endif -%}
  {% endfor %}

{%- else -%}
<!-- Display projects without categories -->

{%- assign sorted_projects = site.projects | sort: "importance" -%}
  <!-- Generate cards for each project -->

{% if page.horizontal -%}
  <div class="container">
    <div class="row row-cols-2">
    {%- for project in sorted_projects -%}
      {% include projects_horizontal.html %}
    {%- endfor %}
    </div>
  </div>
  {%- else -%}
  <div class="grid">
    {%- for project in sorted_projects -%}
      {% include projects.html %}
    {%- endfor %}
  </div>
  {%- endif -%}
{%- endif -%}
</div>
{% endcomment %}
