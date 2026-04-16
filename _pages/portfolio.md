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
    {% unless post.tags contains 'featured' %}
    <div class="portfolio-card">
      {% if post.header.teaser %}
        <a href="{{ post.url | relative_url }}">
          <img src="{{ post.header.teaser | relative_url }}" alt="{{ post.title }}">
        </a>
      {% endif %}
      <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
      {% if post.excerpt %}
        <p>{{ post.excerpt | markdownify | strip_html | truncate: 170 }}</p>
      {% endif %}
    </div>
    {% endunless %}
  {% endfor %}
</div>

## Modeling and Simulation
<div class="portfolio-grid">
  {% assign entries = site.portfolio | where_exp: "item", "item.categories contains 'Modeling-Simulation'" | sort: "date" | reverse %}
  {% for post in entries %}
    {% unless post.tags contains 'featured' %}
    <div class="portfolio-card">
      {% if post.header.teaser %}
        <a href="{{ post.url | relative_url }}">
          <img src="{{ post.header.teaser | relative_url }}" alt="{{ post.title }}">
        </a>
      {% endif %}
      <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
      {% if post.excerpt %}
        <p>{{ post.excerpt | markdownify | strip_html | truncate: 170 }}</p>
      {% endif %}
    </div>
    {% endunless %}
  {% endfor %}
</div>

## Image & Signal Processing and Machine Learning
<div class="portfolio-grid">
  {% assign entries = site.portfolio | where_exp: "item", "item.categories contains 'image-data-analysis'" | sort: "date" | reverse %}
  {% for post in entries %}
    {% unless post.tags contains 'featured' %}
    <div class="portfolio-card">
      {% if post.header.teaser %}
        <a href="{{ post.url | relative_url }}">
          <img src="{{ post.header.teaser | relative_url }}" alt="{{ post.title }}">
        </a>
      {% endif %}
      <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
      {% if post.excerpt %}
        <p>{{ post.excerpt | markdownify | strip_html | truncate: 170 }}</p>
      {% endif %}
    </div>
    {% endunless %}
  {% endfor %}
</div>
