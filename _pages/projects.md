---
title: "Projects"
layout: single
permalink: /projects/
toc: false
---

Open source work across endpoint management, security tooling, infrastructure automation, and enterprise IT.

## Personal Projects

{% assign personal = site.data.projects.personal %}
{% for project in personal %}
### [{{ project.name }}]({{ project.url }})
{{ project.description }}
{% if project.stars %}⭐ {{ project.stars }} stars{% endif %}{% if project.forks %} · 🍴 {{ project.forks }} forks{% endif %}

**Tags:** {% for tag in project.tags %}`{{ tag }}` {% endfor %}
{% endfor %}

---

## UNT Computing for Arts & Sciences (UNT-CAS)

Work from my time at the University of North Texas, Department of Computing for Arts and Sciences.

{% assign unt = site.data.projects.unt_cas %}
{% for project in unt %}
### [{{ project.name }}]({{ project.url }})
{{ project.description }}
{% if project.stars %}⭐ {{ project.stars }} stars{% endif %}{% if project.forks %} · 🍴 {{ project.forks }} forks{% endif %}

**Tags:** {% for tag in project.tags %}`{{ tag }}` {% endfor %}
{% endfor %}
