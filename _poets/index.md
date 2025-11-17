---
layout: default
title: Poems Collection
permalink: /poems/
---

# Poems Collection

Explore featured poems:

<ul>
{% for poem in site.poems %}
  <li>
    <a href="{{ poem.url | relative_url }}">{{ poem.title }}</a>
    {% if poem.excerpt %} — <small>{{ poem.excerpt }}</small>{% endif %}
  </li>
{% endfor %}
</ul>
