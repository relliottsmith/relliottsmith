---
layout: page
permalink: /publications/
title: publications
description: 
years: [2022, 2019, 2018, Preprint]
nav: true
nav_order: 1
---

{{ page.title }}
================

### papers, math

<!-- _pages/publications.md -->
<div class="publications, math">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>

### papers, other

<!-- _pages/publications.md -->
<div class="publications, other">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f nonmathpapers -q @*[year={{y}}]* %}
{% endfor %}

</div>