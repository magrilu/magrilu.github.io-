---
layout: page
permalink: /publications/
title: publications
description: This material is presented to ensure timely dissemination of scholarly and technical work. Copyright and all rights therein are retained by authors or by other copyright holders.
years: [ 2019, 2018, 2017, 2016, 2015, 2014, 2012]
---

{% for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
