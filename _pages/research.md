---
layout: page
title: Research
permalink: /research/
description:
nav: true
display_categories: [work]
horizontal: false
---

I've been working in the High Performance Computing (HPC) research field since 2010, and in this time I have collaborated widely with other universities, UK and US national laboratories, and industry.
Much of my recent work has been focussed on the performance, portability and programmability of applications of interest to the Plasma Physics community.
These projects have been funded under the ExCALIBUR Fusion Use Case ([Project NEPTUNE](https://excalibur.ac.uk/projects/excalibur-fusion-use-case-project-neptune-neutrals-plasma-turbulence-numerics-for-the-exascale/)) and by EPSRC ([EP/W029111/1](https://gow.epsrc.ukri.org/NGBOViewGrant.aspx?GrantRef=EP/W029111/1)).

Broadly speaking, my research interests fall into three categories:

#### Performance Analysis and Optimisation

* Performance modelling of applications
* Algorithmic optimisations of applications from the science and engineering domains
* Evaluation of novel programming models and architectures

#### Parallel File Systems and I/O

* Tracing and analysis of I/O in parallel applications
* Optimisation of I/O operations on parallel file systems
* Replication of sensitive I/O patterns in open environments

#### Energy-aware Computation

* Analysis and modelling of energy consumption for parallel applications
* Energy-aware optimisation of applications

## PhD Opportunities

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