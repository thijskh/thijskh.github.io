---
layout: archive
permalink: /columns/
title: "Columns"
author_profile: true
taxonomy: categories
---

## Mijn laatste vijf columns

{% for post in site.posts limit:5 %}
<h3><a href="{{post.url}}">{{post.title}}</a> ({%- include date-nl.html date=post.date -%})</h3>

{{post.excerpt}} <a href="{{post.url}}">(lees verder)</a>

{% endfor %}

## Alle columns per categorie

{% assign categories = site.data.taxonomy['categories'] %}
{% for category in categories %}
* **[{{category.title}}]({{site.categories[category].url}})**
{% endfor %}
