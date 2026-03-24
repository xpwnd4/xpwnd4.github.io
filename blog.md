---
layout: default
title: Blog
permalink: /blog/
---
<section class="panel">
  <h2>Blog Posts</h2>
  <ul class="card-list">
    {% for post in site.posts %}
      <li>
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
        <span class="meta">— {{ post.date | date: "%B %d, %Y" }}</span>
      </li>
    {% endfor %}
  </ul>
</section>
