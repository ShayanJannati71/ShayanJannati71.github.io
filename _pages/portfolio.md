---
title: "Portfolio"
layout: single
permalink: /portfolio/
classes: wide
---

## Fabrication
<div class="entries-grid">
  {% assign entries = site.portfolio
     | where_exp: "item", "item.categories contains 'fabrication'"
     | sort: "date" | reverse %}
  {% for post in entries %}
    {% include archive-single.html type="grid" %}
  {% endfor %}
</div>

## Image & Data Analysis
<div class="entries-grid">
  {% assign entries = site.portfolio
     | where_exp: "item", "item.categories contains 'image-analysis'"
     | sort: "date" | reverse %}
  {% for post in entries %}
    {% include archive-single.html type="grid" %}
  {% endfor %}
</div>




