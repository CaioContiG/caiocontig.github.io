---
layout: page
title: Projects
permalink: /Projects/
description: Main projects and activities participated. Click on each project to explore more details.
nav: true
nav_order: 2
#display_categories: [work, fun]
horizontal: false
---

<!-- pages/projects.md -->
<!-- CURRENT PROJECTS -->
<div class="projects">
<h3 style="font-family: 'Your Font', sans-serif;">Current</h3>{%- if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized projects -->
  {%- for category in page.display_categories %}
    {%- if category == "current" %}
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
    {%- endif %}
  {% endfor %}
{%- else -%}
<!-- Display projects without categories -->
  {%- assign sorted_projects = site.projects | where: "category", "current" | sort: "importance" -%}
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


<!-- PREVIOUS PROJECTS -->
<div class="projects">
<h3 style="font-family: 'Your Font', sans-serif;">Previous</h3>
{%- if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized projects -->
  {%- for category in page.display_categories %}
    {%- if category == "previous" %}
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
    {%- endif %}
  {% endfor %}
{%- else -%}
<!-- Display projects without categories -->
  {%- assign sorted_projects = site.projects | where: "category", "previous" | sort: "importance" -%}
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
