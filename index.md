---
layout: home
title: Home
---

# Hey, I'm Dan.

Data Scientist & AI Engineer based in London. I build production ML systems, LLM agents, and apps that solve real problems. Currently Operational Data Lead at TRUSS.

## Projects

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
