---
title: "Portfolio"
layout: single
permalink: /portfolio/
classes: wide
---

## Featured Project

<div class="portfolio-grid featured-grid">
  {% assign featured = site.portfolio | where_exp: "item", "item.tags contains 'featured'" %}
  {% for post in featured limit:1 %}
    <div class="portfolio-card featured">

      {% if post.header.teaser %}
        <a href="{{ post.url | relative_url }}">
          <img src="{{ post.header.teaser | relative_url }}" alt="{{ post.title }}">
        </a>
      {% endif %}

      <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>

      {% if post.excerpt %}
        <p>{{ post.excerpt | strip_html }}</p>
      {% endif %}

    </div>
  {% endfor %}
</div>

## Device Fabrication & Development
<div class="portfolio-grid">
  {% assign entries = site.portfolio | where_exp: "item", "item.categories contains 'fabrication'" | sort: "date" | reverse %}
  {% for post in entries %}
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
  {% endfor %}
</div>

## Modeling and Simulation
<div class="portfolio-grid">
  {% assign entries = site.portfolio | where_exp: "item", "item.categories contains 'Modeling-Simulation'" | sort: "date" | reverse %}
  {% for post in entries %}
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
  {% endfor %}
</div>

## Image & Signal Processing and Machine Learning
<div class="portfolio-grid">
  {% assign entries = site.portfolio | where_exp: "item", "item.categories contains 'image-data-analysis'" | sort: "date" | reverse %}
  {% for post in entries %}
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
  {% endfor %}
</div>
