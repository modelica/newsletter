---
index: true
hidden: true
layout: default
title: "Some articles missing? v5"
name: "2018-01"
---
{% assign pages = site.[page.name] %}

{% for page in pages %}
{% assign valid = (page.index or page.category="association" or page.category="vendor") %}
. {{ page.path }} is {{ valid }} {% if valid %} is valid {% endif %}

{% unless page.index %} 
{% if page.category !="association" and page.category != "vendor" or page.category != "library" or page.category != "project" or page.category != "association") %}
- Kaboom! [{{ page.title }}]({{ page.path }}) {% if page.hidden %} *Hidden* {% endif %}
{% else %}
- {{ page.path }} ok...
{% endif %}
{% endunless %}
{% endfor %}
