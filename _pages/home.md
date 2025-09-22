---
layout: home
title: "Home"
permalink: /
hero:
  image: "/assets/images/Portfolio_Picture.jpeg"   # optional profile or background image
  tagline: "Ph.D. in Mechanical Engineering | Biomedical Devices & Mechatronics"
  cta_text: "View My Projects"
  cta_link: "/portfolio/"
---

# About Me

Hi, I'm **Shayan Jannati**, a Ph.D. graduate in Mechanical Engineering (UBC), specializing in **biomedical devices, hiPSC-CM research, and mechatronics**.  
Check out my [projects portfolio](/portfolio/) to see my work.

---

# My Projects

Below are some of my recent projects. Click any project to see details:

<ul>
  {% for project in site.portfolio %}
    <li>
      <a href="{{ project.url }}">{{ project.title }}</a>
      {% if project.excerpt %}
        - {{ project.excerpt }}
      {% endif %}
    </li>
  {% endfor %}
</ul>

