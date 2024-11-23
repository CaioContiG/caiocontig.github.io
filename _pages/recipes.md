---
layout: page
title: Recipes
permalink: /recipes/
description: I also enjoy cooking! Here are some of my recipes. Be aware they might change as I tweak and improve them over time.
nav: true
nav_order: 2
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
      {%- assign categorized_projects = site.recipes | where: "category", category -%}
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
  {%- assign sorted_projects = site.recipes | where: "category", "current" | sort: "importance" -%}
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