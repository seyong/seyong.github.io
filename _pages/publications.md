---
layout: page
permalink: /publications/
title: Publication
description: Tags denote keywords of my participation in the paper.
years: [2019,2018,2017,2016,2014,2013]
nav: true
---

<div class="publications">
  {% for y in page.years %}
    <h2 class="year">{{y}}</h2>
    {% bibliography -f papers -q @*[year={{y}}]* %}
  {% endfor %}
</div>
