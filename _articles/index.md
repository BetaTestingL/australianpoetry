---
layout: default
title: Articles
permalink: /articles/
---

# Articles

<ul>
{% assign articles = site.categories.articles %}
{% for post in articles %}
  <li>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    <small> — {{ post.date | date: "%b %-d, %Y" }}</small>
  </li>
{% endfor %}
</ul>
