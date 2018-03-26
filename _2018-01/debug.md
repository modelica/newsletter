---
index: true
hidden: true
layout: default
title: "Some articles missing? v7"
name: "2018-01"
---

{% assign name = page.name %}

{% for page in site.[name] %}
{% if page.index != true %}
{% if page.category != "association" and page.category != "vendor" and page.category != "library" %}
* error at {{ page.path }} {% if page.hidden %} HIDDEN {% endif %}
{% endif %}
{% endif %}
{% endfor %}
