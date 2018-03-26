---
index: true
hidden: true
layout: default
title: "Some articles missing? v7"
name: "2018-01"
---
{% assign pages = site.[page.name] %}
{% for page in pages %}

{% if page.category !="association" and page.category != "vendor" and page.category != "library" and page.category != "project" and page.category != "association" %}


- {{ page.path }} ok...


{% endfor %}
