---
layout: default
title: Projects
permalink: /projects/
---

# projects

{% for project in site.projects %}
## [{{ project.title }}]({{ project.url }})

{{ project.content }}

---
{% endfor %}
