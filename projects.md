---
layout: default
title: Projects
permalink: /projects/
---

<h2>Projects</h2>
<ul class="project-list">
  {% for project in site.data.projects %}
  <li>
    <span class="project-meta">{{ project.date | date: "%b %-d, %Y" }}</span>
    <h2>
      <a class="project-link" href="{{ project.url | prepend: site.baseurl }}">{{ project.title }}</a>
    </h2>
    <p class="project-description">{{ project.description }}</p>
  </li>
  {% endfor %}
</ul>
