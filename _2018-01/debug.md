---
index: true
hidden: true
layout: default
title: "Some articles missing? v7"
name: "2018-01"
---
{% assign pages = site.[page.name] %}
{% for page in pages %}

{% if page.category !="association" and page.category != "vendor" and page.category != "library" and page.category != "project" and page.category != "association") %}

{% if page.index %}
- {{ page.path }} is INDEX {% if page.hidden %} *Hidden* {% endif %}
{% else %}
- ERROR! [{{ page.title }}]({{ page.path }}) {% if page.hidden %} *Hidden* {% endif %}
{% endif %}

{% else %}
- {{ page.path }} ok...
{% endif %}


{% endfor %}
