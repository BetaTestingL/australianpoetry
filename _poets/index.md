---
layout: default
title: Poets Directory
permalink: /poets/
---

# Australian Poets Directory

Below is a curated list of poets featured on this site. Click a name to read short bio and works.

<ul>
{% for poet in site.poets %}
  <li>
    <a href="{{ poet.url | relative_url }}">{{ poet.title }}</a>
    {% if poet.excerpt %} — <small>{{ poet.excerpt }}</small>{% endif %}
  </li>
{% endfor %}
</ul>
