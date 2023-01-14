---
layout: base
title: Under konstruktion
pagination:
  data: collections.posts
  size: 2
  alias: posts
---

Denna sida kommer så småningom vara mer intressant…

## Alla inlägg hitils

{%- for post in collections.posts %}
- [{{ post.data.title }}]({{ post.url }})
    {%- endfor %}

{% if pagination.href.previous %}
  <a href="{{pagination.href.next}}">Nästa sida</a>
{% endif %}
