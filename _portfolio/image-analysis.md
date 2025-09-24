---
title: "Image & Data Analysis"
layout: none
permalink: /portfolio/image-analysis/
---


<div class="entries-grid">
  {% assign entries = site.portfolio | where_exp: "item", "item.categories contains 'image-analysis'" %}
  {% for post in entries %}
    {% include archive-single.html type="grid" %}
  {% endfor %}
</div>
