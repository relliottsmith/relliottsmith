---
layout: page
permalink: /publications/
title: Publications
description: 
years1: [2022, in prep]
years2: [2019,2018]
nav: true
nav_order: 1
---

### Math

<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years1 %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>

### Other

<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years2 %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f nonmathpapers -q @*[year={{y}}]* %}
{% endfor %}

</div>