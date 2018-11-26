{% include build_email_list_category.md section="Modelica Association" category="association" %}
{% include build_email_list_category.md section="Related projects" category="project" %}
{% include build_email_list_category.md section="Vendor news" category="vendor" %}
{% include build_email_list_category.md section="News from libraries" category="library" %}
{% include build_email_list_category.md section="Conferences and user meetings" category="conference" %}
{% include build_email_list_category.md section="Education news" category="education" %}
    
{% assign cats = "association,project,vendor,library,conference,education" %}
{{ cats }} __ and __ {{ page.category }}

 
{% for page in site.[name] %}
{% if page.index != true and hidden != true and page.category != "association" and page.category != "project" and page.category != "vendor" and page.category != "library" and page.category != "conference" and page.category != "education" %}
* ERROR: [{{ page.title }}]({{site.url}}/{{ name }}/index.html#{{ page.title | slugify }}) uncategorized!
* sumuturhERROR: [{{ page.name }}]({{page.url}}) uncategorized!

{% unless cats contains page.category  %}
sum stuff
{% endunless %}

{% endif %}
{% endfor %}
