---
layout: archive
permalink: /columns/
title: "Columns"
author_profile: true
---

## Mijn laatste vijf columns

{% for post in site.posts limit:5 %}
<h3><a href="{{post.url}}">{{post.title}}</a> ({%- include date-nl.html date=post.date -%})</h3>

{{- post.excerpt -}} <small><a href="{{post.url}}">(lees verder)</a></small>
{% endfor %}

## Alle columns per categorie

* **[De coronacrisis]({{site.categories['Corona'].url}})**
* **[Het academisch bedrijf]({{site.categories['Academisch-bedrijf'].url}})**
* **[Geboorte & dood]({{site.categories['Geboorte-dood'].url}})**
* **[Van alles en nog wat]({{site.categories['Alles-nogwat'].url}})**
