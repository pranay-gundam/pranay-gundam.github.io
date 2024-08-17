---
layout: page
permalink: /work/
title: My Work
description: Writing well written and organized code is a particular passion of mine and something that I think is drastically needed in the field of econ. I've put a few of the repos that I'm especially proud of here but feel free to checkout my github for all of my projects. On the economics side I am primarily interested in spatial general equilibrium models and other macro models to study monetary policy.
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
