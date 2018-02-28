{% assign name = page.name %}
{% assign cat = include.category %}
{% assign section  = include.section %}

### {{ section }}
{% for page in site.[name] %}
{% if page.category == cat and page.index != true and hidden != true %}
* [{{ page.title }}]({{site.url}}/{{ name }}/index.html#{{ page.title | slugify }})
{% endif %}
{% endfor %}
