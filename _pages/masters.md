---
title: "Graduate Studies"
layout: single
permalink: /masters/
toc: true
toc_label: "Courses"
author_profile: true
---

## Master of Science — Learning Technologies
**University of North Texas** | Department of Learning Technologies

Coursework exploring instructional design, educational technology, and the intersection of learning science with modern tools. Blog posts and reflections from each course are preserved below.

### Courses

| Course | Title |
|--------|-------|
| **LTEC 5200** | Foundations of Learning Technologies |
| **LTEC 5210** | Introduction to Learning Technologies |
| **LTEC 5220** | Learning and Technology |
| **LTEC 5240** | Technology and Learning Environments |
| **LTEC 5510** | Instructional Design |
| **LTEC 6010** | Advanced Topics in Learning Technologies |
| **LTEC 6800** | Research in Learning Technologies *(2022)* |

> Posts from these courses were originally hosted at their own subdomains (e.g., `ltec6800.ray.pillers.us`). Those subdomains now redirect here.

---

## Course Posts

{% assign masters_posts = site.posts | where_exp: "post", "post.tags contains 'masters'" %}
{% if masters_posts.size > 0 %}
  {% assign grouped = masters_posts | group_by: "categories" %}
  {% for group in grouped %}
### {{ group.name }}
    {% for post in group.items %}
- [{{ post.title }}]({{ post.url | relative_url }}) <small>{{ post.date | date: "%B %d, %Y" }}</small>
    {% endfor %}
  {% endfor %}
{% else %}
*No posts found — check that posts are tagged `masters`.*
{% endif %}
