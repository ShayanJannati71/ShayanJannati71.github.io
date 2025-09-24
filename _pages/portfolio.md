---
title: "Portfolio"
layout: single
permalink: /portfolio/
classes: wide
---

{% assign fabrication_entries = site.portfolio
   | where_exp: "item", "item.categories contains 'fabrication'"
   | sort: "date" | reverse %}
{% include archive.html title="Fabrication" type="grid" entries=fabrication_entries %}

{% assign analysis_entries = site.portfolio
   | where_exp: "item", "item.categories contains 'image-analysis'"
   | sort: "date" | reverse %}
{% include archive.html title="Image & Data Analysis" type="grid" entries=analysis_entries %}
