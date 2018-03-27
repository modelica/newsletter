---
title: Modelica Association Newsletters
layout: default
mainpage: true
---

The [Modelica Association] newsletter informs the audience about all topics covered by the Modelica Association (Modelica language, FMI, SSP), libraries, related projects and tools and news in education (courses, books and related materials). You can [subscribe](http://eepurl.com/dpvVdH) to receive the newsletter as well.

<!-- Begin MailChimp Signup Form -->
<link href="//cdn-images.mailchimp.com/embedcode/horizontal-slim-10_7.css" rel="stylesheet" type="text/css">
<style type="text/css">
	#mc_embed_signup{background:#fff; clear:left; font:14px Helvetica,Arial,sans-serif; width:100%;margin:2em}
	/* Add your own MailChimp form style overrides in your site stylesheet or in this style block.
	   We recommend moving this block and the preceding CSS link to the HEAD of your HTML file. */
</style>
<div id="mc_embed_signup">
<form action="https://creativeconnections.us12.list-manage.com/subscribe/post?u=0be901f875b69817eddd7e71b&amp;id=0cb2cf5b72" method="post" id="mc-embedded-subscribe-form" name="mc-embedded-subscribe-form" class="validate" target="_blank" novalidate>
    <div id="mc_embed_signup_scroll">
	<label for="mce-EMAIL">Subscribe to our mailing list</label>
	<input type="email" value="" name="EMAIL" class="email" id="mce-EMAIL" placeholder="email address" required>
    <!-- real people should not fill this in and expect good things - do not remove this or risk form bot signups-->
    <div style="position: absolute; left: -5000px;" aria-hidden="true"><input type="text" name="b_0be901f875b69817eddd7e71b_0cb2cf5b72" tabindex="-1" value=""></div>
    <div class="clear"><input type="submit" value="Subscribe" name="subscribe" id="mc-embedded-subscribe" class="button"></div>
    </div>
</form>
</div>

<!--End mc_embed_signup-->
    
Contributions are open to everyone, please see the [submission guidelines](submission-guidelines.html) for details.

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

Below is an archive of old newsletters.

* [2015-01](archives/2015-01.html)
