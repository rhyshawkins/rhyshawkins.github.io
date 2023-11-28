---
layout: page
title: projects
permalink: /projects/
description: Currently available projects for students
nav: true
nav_order: 2
display_categories: [undergrad, phd]
horizontal: false
---

I have a keen interest in providing student projects that apply new and developing computer
science approaches to scientific problems in the Earth Sciences. You can find potential student
projects below. If you have a project in mind that you're passionate about that involves
Computation and Earth Sciences, then please feel free to contact me and I'd happy to chat and/or
put you in touch with the right people.


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

<h2 class="category">Past Projects</h2>


<div class="publications">

<h2 class="year"> 2023 </h2>

<ul>
<li> Heming Zhu, <emph> "Application and performance analysis of Soft Spectral Element Method in Wave Simulations" </emph> (COMP4550), co-supervised with Quanling Deng </li>
</ul>

<ul>
<li> Xuzeng He, <emph> "Unleashing the power of Machine Learning in Geodynamics" </emph> (COMP4560), co-supervised with Alberto F. Martin and Sia Ghelichkhan </li>
</ul>

<ul>
<li> Raymond Horley, <emph> "Deep learning techniques for seasonal climate forecasts in Australia" </emph> (COMP3770) co-supervised with Warren Jin (CSIRO) </li>
</ul>

<ul>
<li> Muhammad Sulthan Mazaya, <emph> "Optimisation and integration of geodynamic forward models into a Bayesian Trans-dimensional framework" </emph>, (FRT Scholar), co-supervised with Sia Ghelichkhan and Mark Hoggard </li>
</ul>

<ul>
<li> Ishan Tandon, <emph> "Bayesian Trans-dimensional inversion of geodynamics observations" </emph>, (FRT Scholar)
, co-supervised with Sia Ghelichkhan and Mark Hoggard </li>
</ul>

<ul>
<li> Porntipa Poonpolsub, "Curvelet wavefield partitioning of DAS observations", (Summer Scholar), co-supervised with Voon Hui Lai and Meghan Miller </li>
</ul>

<ul>
<li> Lin Xi, "Curvelet wavefield partitioning of DAS observations", (Summer Scholar), co-supervised with Voon Hui Lai and Meghan Miller </li>
</ul>

</div>