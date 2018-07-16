{% assign name = page.name %}
{% assign cat = include.category %}
{% assign section  = include.section %}

{% assign cat_posts = ((site.[name] | where:"category", cat | sort:"date" | reverse %}

{% if cat_posts.size > 0 and cat != "letter" %}
# {{ section }}
{% endif %}

{% for page in cat_posts %}
{% unless page.hidden or page.index %}
## {{ page.title }} 
{#{{ page.title | slugify }}}

#### Hey 
{: #{{ page.title | slugify }}}

#### Ho 
{: #id key="{{ page.title | slugify }}"}
{{ page.content | markdownify }}
{% if page.author %}
*This article is provided by {{ page.author }}*  
{% endif %}

***

{% endunless %}
{% endfor %}
