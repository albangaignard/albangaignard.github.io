---
layout: page
permalink: /publications/
title: publications
description: Here are reported my last 5-years publications. A more complete list can be found in [HAL](https://cv.hal.science/alban-gaignard).  
years: [2023,2022,2021,2020,2019]
nav: true
nav_order: 2
---

<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>