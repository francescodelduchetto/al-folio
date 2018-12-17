---
layout: page
permalink: /publications/
title: publications
description: Publications by categories in reversed chronological order.
years: [2018, 2017, 2015]
social: true
---

{% bibliography %}

{% comment %}
{% for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
{% endcomment %}
