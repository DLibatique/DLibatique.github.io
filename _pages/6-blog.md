---
layout: page
title: Blog
permalink: /blog
---

{% for post in site.posts %}
  * <strong>{{ post.date | date_to_string }}</strong> &raquo; [ {{ post.title }} ]({{ post.url }})
  {% if post.excerpt %}
    <small>{{ post.excerpt }}</small>
  {% endif %}
{% endfor %}
