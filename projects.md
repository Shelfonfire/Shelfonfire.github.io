---
layout: page
title: Projects
permalink: /projects/
---

# Projects

Things I've built — shipping fast and learning as I go.

<div class="project-cards">
{% for project in site.projects reversed %}
<div class="project-card">
  <h3><a href="{{ project.url }}">{{ project.title }}</a></h3>
  <p>{{ project.description }}</p>
  <div class="project-tech">{{ project.technologies }}</div>
  <div class="project-links">
    {% if project.demo %}<a href="{{ project.demo }}" class="btn" target="_blank">Live Demo</a>{% endif %}
    {% if project.github %}<a href="{{ project.github }}" class="btn btn-outline" target="_blank">GitHub</a>{% endif %}
    <a href="{{ project.url }}" class="btn btn-outline">Details</a>
  </div>
</div>
{% endfor %}
</div>
