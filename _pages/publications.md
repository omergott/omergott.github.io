---
layout: page
permalink: /publications/
title: publications
description:
conference_years: [2021, 2020, 2019, 2018, 2017, 2015, 2014, 2012]
workshop_years: [2021, 2020, 2019, 2018]
nav: true
---

<div class="publications">
<h3>Conference and Journal Papers</h3>
{% for y in page.conference_years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>

<div class="publications">
<h3>Workshops and Preprints</h3>
{% for y in page.workshop_years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f workshops -q @*[year={{y}}]* %}
{% endfor %}

</div>

