---
layout: page
permalink: /publications/
title: Publications
description: 
status: [preprint, in prep]
years2: [2019,2018]
nav: true
nav_order: 1
---

### Math

<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.status %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[status={{y}}]* %}
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