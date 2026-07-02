---
layout: no-header
title: Notes
permalink: /notes/
---

# Notes

A collection of thoughts, ideas, and observations.

{% for post in site.posts %}
  {% if post.categories contains 'notes' %}
  - [{{ post.title }}]({{ post.url }}) — {{ post.date | date: "%B %d, %Y" }}
  {% endif %}
{% endfor %}
