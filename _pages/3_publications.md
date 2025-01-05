---
layout: page
permalink: /publications/
title: Publications
description: Publications by categories in reversed chronological order.
years: [2024, 2023, 2022, 2021, 2020, 2019, 2018, 2016, 2013, 2011, 2010, 2007]
---

{% for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
