---
layout: page
permalink: /projects/
title: projects
description: I hope this page gets more crowded along the way...
years: [2023, 2021]

nav: true
nav_order: 1
---
<!-- _pages/projects.md -->
<div class="projects">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
