---
layout: default
title: Articles
permalink: /articles/
---

# Articles

Latest articles and guides:

<ul>
{% assign posts = site.posts | where_exp: "post", "post.categories contains 'articles' or post.layout == 'post'" %}
{% for post in posts %}
  <li>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    <small> — {{ post.date | date: "%b %-d, %Y" }}</small>
  </li>
{% endfor %}
</ul>
