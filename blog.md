---
layout: blog-layout.liquid
title: Blog

pagination:
  data: collections.post
  size: 2
  alias: posts
---

Blog page

<ul>
{% for post in posts %}
<li>
 <a href="{{post.url}}">{{post.data.title}} </a> - <em>{{ post.date | date: "%Y-%m-%d" }}</em>

</li>
{% endfor %}

</ul>
{% if pagination.href.previous %}
<a href="{{ pagination.href.previous }}">Previous Page</a>
{% endif %}

{% if pagination.href.next %}
<a href="{{ pagination.href.next }}">Next Page</a>
{% endif %}
