---
layout: page
permalink: /publications/
title: Publications
description: A list of my publications.
years: [2021,2019,2017]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
