{% assign name = page.collection %}
{% assign cat = include.category %}
{% assign section  = include.section %}
{% assign cat_posts = ((site.[name] | where:"category", cat | sort:"date" | reverse %}

{% if cat_posts.size > 0 and cat != "letter" %}
### {{ section }}
{% endif %}

{% for page in cat_posts %}
{% if page.category == cat and page.index != true and hidden != true %}
* [{{ page.title }}]({{site.url}}/{{ name }}/index.html#{{ page.title | slugify }})
{% endif %}
{% endfor %}
