---
title: "Fabrication"
permalink: /portfolio/fabrication/
layout: grid
---

<div class="entries-grid">
  {% assign entries = site.portfolio | where_exp: "item", "item.categories contains 'fabrication'" %}
  {% for post in entries %}
    {% include archive-single.html type="grid" %}
  {% endfor %}
</div>
