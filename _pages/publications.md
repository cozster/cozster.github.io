---
layout: page
permalink: /publications/
title: publications
description: Selected publications in reverse chronological order.
years: [2023, 2021, 2019, 2018, 2014, 2013, 2012, 2011]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
