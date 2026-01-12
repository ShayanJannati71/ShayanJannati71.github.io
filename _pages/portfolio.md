---
title: "Portfolio"
layout: single
permalink: /portfolio/
classes: wide
---

## Device Fabrication & Development
<div class="entries-grid">
  {% assign entries = site.portfolio | where_exp: "item", "item.categories contains 'fabrication'" | sort: "date" | reverse %}
  {% for post in entries %}
    {% include archive-single.html type="grid" %}
  {% endfor %}
</div>

<div style="clear: both;"></div>   <!-- force new row -->

## Modeling and Simulation
<div class="entries-grid">
  {% assign entries = site.portfolio | where_exp: "item", "item.categories contains 'Modeling-Simulation'" | sort: "date" | reverse %}
  {% for post in entries %}
    {% include archive-single.html type="grid" %}
  {% endfor %}
</div>

## Image & Signal Processing and Machine Learning
<div class="entries-grid">
  {% assign entries = site.portfolio | where_exp: "item", "item.categories contains 'image-data-analysis'" | sort: "date" | reverse %}
  {% for post in entries %}
    {% include archive-single.html type="grid" %}
  {% endfor %}
</div>

