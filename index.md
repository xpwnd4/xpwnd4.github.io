---
layout: default
title: Home
---
<section class="hero panel">
  <p class="terminal-line">xpwnd4@security:~$ ls -la portfolio/</p>
  <h2>Cybersecurity writeups, projects, labs, and research.</h2>
  <p>This site is built for technical blogging, writeups, project showcases, and educational resources with a cleaner hacker-style aesthetic.</p>
  <p>
    <a href="/writeups/">[ Browse Writeups ]</a>
    <a href="/projects/">[ View Projects ]</a>
    <a href="/blog/">[ Read Blog ]</a>
  </p>
</section>

<section class="panel">
  <h2>Recent Blog Posts</h2>
  <ul class="card-list">
  {% for post in site.posts limit:3 %}
    <li><a href="{{ post.url | relative_url }}">{{ post.title }}</a> <span class="meta">— {{ post.date | date: "%b %d, %Y" }}</span></li>
  {% endfor %}
  </ul>
</section>

<section class="panel">
  <h2>Featured Writeups</h2>
  <ul class="card-list">
  {% for item in site.writeups limit:3 %}
    <li><a href="{{ item.url | relative_url }}">{{ item.title }}</a></li>
  {% endfor %}
  </ul>
</section>

<section class="panel">
  <h2>Featured Projects</h2>
  <ul class="card-list">
  {% for item in site.projects limit:2 %}
    <li><a href="{{ item.url | relative_url }}">{{ item.title }}</a></li>
  {% endfor %}
  </ul>
</section>
