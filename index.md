---
title: Modelica newsletters archive
layout: default
---

Hello world! This is a newsletter archive.

Please contribute! See [submission guidelines](submission-guidelines.html)


## Newsletters
here is the sorted set of all sample pages:

  
  <section>
    <ul> 
{% assign sorted = (site.collections | sort: 'date') | reverse %}
         
{% for collection in sorted %}

  {% assign name = collection.label %}
  {% unless name == "posts" %}
      
    {% for page in site.[name] %}
    {% if page.index == true and page.hidden != true %}
      <li><a href="{{ page.url | prepend: site.baseurl }}">{{ page.title }}</a><BR />{{ page.description }}</li>
    {% endif %}
    {% endfor %}
{% endunless %}
{% endfor %}    
    </ul>
  </section>


## Archives

Below is a archive of old newsletters.

* [2015-01](archives/2015-01.html)
