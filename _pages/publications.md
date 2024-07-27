---
layout: page
permalink: /work/
title: My Work
description: An intro about your research interests.
nav: true
nav_order: 3
display_categories: [work]

---

<!-- _pages/publications.md -->
<div class="publications">

<h2>Projects</h2>
{% for category in page.display_categories %}
  {% assign categorized_projects = site.projects | where: "category", category %}
  {% assign sorted_projects = categorized_projects | sort: "importance" %}
  <!-- Generate cards for each project -->
    {% for project in sorted_projects %}
      {% include projects.liquid %}
    {% endfor %}
  {% endfor %}

<br />
<br />
<h2>Papers</h2>
{% bibliography %}

<br />
<br />

</div>
