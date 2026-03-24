---
layout: default
title: Resources
permalink: /resources/
---
<section class="panel">
  <h2>Resources</h2>
  <ul class="card-list">
    {% for item in site.resources %}
      <li><a href="{{ item.url | relative_url }}">{{ item.title }}</a></li>
    {% endfor %}
  </ul>
</section>
