---
layout: archive
permalink: /columns/
title: "Columns"
author_profile: true
---

Mijn laatste vijf columns:

{% for post in site.posts limit:5 %}
[{{post.title}}]({{post.url}}) ({%- include date-nl.html date=post.date -%})

{{post.excerpt}}

{% endfor %}

Bekijk alle columns hier per categorie:

<ul>
{% for category in site.categories %}
    <li><a href="{{category.url}}"><strong>{{category|first}}</strong></a></li>
{% endfor %}
</ul>
