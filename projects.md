---
layout: default
title: Projects
permalink: /projects/
---

<div class="projects-wrap">
  <h1>projects</h1>

  {% for project in site.projects %}
    <div class="project-item">
      <h2>{{ project.title }}</h2>
      <p>{{ project.content | strip_html | strip }}</p>
    </div>
  {% endfor %}
</div>
