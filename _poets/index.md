---
layout: default
title: Poems Collection
permalink: /poems/
---

## Buy Books by {{ page.title }}

Looking for works by {{ page.title }}? Find recommended titles and anthologies on Amazon:

<a class="btn-aff" href="https://www.amazon.com/s?k={{ page.title | uri_escape }}+poems&tag=anubhavp05-21" target="_blank" rel="noopener">Buy books by {{ page.title }}</a>

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
