---
layout: default
title: Projects
permalink: /projects/
---
<section class="panel">
  <h2>Projects</h2>
  <ul class="card-list">
    {% for item in site.projects %}
      <li><a href="{{ item.url | relative_url }}">{{ item.title }}</a></li>
    {% endfor %}
  </ul>
</section>
