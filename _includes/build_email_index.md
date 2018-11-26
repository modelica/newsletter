{% include build_email_list_category.md section="Modelica Association" category="association" %}
{% include build_email_list_category.md section="Related projects" category="project" %}
{% include build_email_list_category.md section="Vendor news" category="vendor" %}
{% include build_email_list_category.md section="News from libraries" category="library" %}
{% include build_email_list_category.md section="Conferences and user meetings" category="conference" %}
{% include build_email_list_category.md section="Education news" category="education" %}
    
{% assign cats = "association,project,vendor,library,conference,education" %}
 
{% for page in site.[name] %}
{% if page.index != true and hidden != true and page.category != "letter" %}
{% unless cats contains page.category  %}
* ERROR: [{{ page.title }}](https://github.com/modelica/newsletter/blob/master/{{ page.path }}) uncategorized! *{{ page.category }}* unknown.
{% endunless %}
{% endif %}
{% endfor %}
