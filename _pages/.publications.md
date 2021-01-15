---
layout: page
permalink: /publications/
title: Publications
description: Currently nothing. Hopefully there will be something in 2021.
years: [2020]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
