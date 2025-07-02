---
layout: page
permalink: /publications/
title: publications
description: Last 5-years publications, an up-to-date list can be found in [HAL](https://cv.hal.science/alban-gaignard).  
years: [2025,2024,2023,2022,2021]
nav: true
nav_order: 2
---

<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>