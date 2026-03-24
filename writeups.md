---
layout: default
title: Writeups
permalink: /writeups/
---
<section class="panel">
  <h2>Writeups</h2>
  <ul class="card-list">
    {% for item in site.writeups %}
      <li><a href="{{ item.url | relative_url }}">{{ item.title }}</a></li>
    {% endfor %}
  </ul>
</section>
