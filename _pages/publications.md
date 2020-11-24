---
layout: page
permalink: /publications/
title: publications
nav_title: publications
description: peer-reviewed manuscripts
years: [2021, 2020, 2019, 2017]
nav: true
---

{% include pubs.html title="Summary per year" source=site.data.pubs-per-year %} 

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
