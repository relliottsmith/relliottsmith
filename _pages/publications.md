---
layout: page
permalink: /publications/
title: publications
description: 
years1: [2022, Preprint]
years2: [2019,2018]
nav: true
nav_order: 1
---

### math

<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years1 %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>

### other

<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years2 %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f nonmathpapers -q @*[year={{y}}]* %}
{% endfor %}

</div>