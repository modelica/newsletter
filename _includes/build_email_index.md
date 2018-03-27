You can also [view the web version]({{site.url}}/{{page.collection}}).

{% include build_email_list_category.md section="Letter from the board (Hidden caption)" category="letter" %}
{% include build_email_list_category.md section="Modelica Association" category="association" %}
{% include build_email_list_category.md section="Related projects" category="project" %}
{% include build_email_list_category.md section="Vendor news" category="vendor" %}
{% include build_email_list_category.md section="News from libraries" category="library" %}
{% include build_email_list_category.md section="Education news" category="education" %}

{% assign cat_posts = ((site.[page.collection] | where:"category", "letter" | sort:"date" %}
{% for page in cat_posts %}
{% unless page.hidden or page.index %}
## {{ page.title }}
{{ page.content | markdownify }}
{% if page.author %} *This article is provided by {{ page.author }}*  {% endif %}
{% endunless %}
{% endfor %}

   

*[Read the rest of the newsletter on the web]({{site.url}}/{{page.collection}})*
{: style="text-align: center;"}
