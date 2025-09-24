---
title: "Portfolio"
layout: single
permalink: /portfolio/
classes: wide
---

## Biomedical Device Development
<div class="entries-grid">
  {% assign entries = site.portfolio | where_exp: "item", "item.categories contains 'fabrication'" | sort: "date" | reverse %}
  {% for post in entries %}
    {% include archive-single.html type="grid" %}
  {% endfor %}
</div>

<div style="clear: both;"></div>   <!-- force new row -->

## Image & Data Analysis
<div class="entries-grid">
  {% assign entries = site.portfolio | where_exp: "item", "item.categories contains 'image-data-analysis'" | sort: "date" | reverse %}
  {% for post in entries %}
    {% include archive-single.html type="grid" %}
  {% endfor %}
</div>

## Modeling & Simulation
<div class="entries-grid">
  {% assign entries = site.portfolio | where_exp: "item", "item.categories contains 'Modeling-Simulation'" | sort: "date" | reverse %}
  {% for post in entries %}
    {% include archive-single.html type="grid" %}
  {% endfor %}
</div>

## Signal Processing & Machine Learning
<div class="entries-grid">
  {% assign entries = site.portfolio | where_exp: "item", "item.categories contains 'Signal-Machine-Learning'" | sort: "date" | reverse %}
  {% for post in entries %}
    {% include archive-single.html type="grid" %}
  {% endfor %}
</div>
