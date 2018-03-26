---
index: true
hidden: true
layout: default
title: "Some articles missing? v7"
name: "2018-01"
---

{% assign name = page.name %}
{% assign cat = include.category %}
{% assign section  = include.section %}

{% for page in site.[name] %}
{% assign inCat = page.category == "association" or page.category == "vendor" or page.category == "library" %}
{% if page.index != true and hidden != true %}
{% unless inCat %}
* {{ page.title }}
{% endunless %}
{% endif %}
{% endfor %}
