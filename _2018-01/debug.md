---
index: true
hidden: true
layout: default
title: "Some articles missing? v7"
name: "2018-01"
---
{% assign pages = site.[page.name] %}
{% for page in pages %}

- {{ page.path }} ok...


{% endfor %}
