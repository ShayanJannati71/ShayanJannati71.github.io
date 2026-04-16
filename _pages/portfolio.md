---
title: "Portfolio"
layout: single
permalink: /portfolio/
classes: wide
---

## Device Fabrication & Development
<div class="portfolio-grid">
  {% assign entries = site.portfolio | where_exp: "item", "item.categories contains 'fabrication'" | sort: "date" | reverse %}
  {% for post in entries %}
    <div class="portfolio-card">
      {% include archive-single.html %}
    </div>
  {% endfor %}
</div>

## Modeling and Simulation
<div class="portfolio-grid">
  {% assign entries = site.portfolio | where_exp: "item", "item.categories contains 'Modeling-Simulation'" | sort: "date" | reverse %}
  {% for post in entries %}
    <div class="portfolio-card">
      {% include archive-single.html %}
    </div>
  {% endfor %}
</div>

## Image & Signal Processing and Machine Learning
<div class="portfolio-grid">
  {% assign entries = site.portfolio | where_exp: "item", "item.categories contains 'image-data-analysis'" | sort: "date" | reverse %}
  {% for post in entries %}
    <div class="portfolio-card">
      {% include archive-single.html %}
    </div>
  {% endfor %}
</div>

