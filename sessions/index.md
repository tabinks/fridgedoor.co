---
layout: page
title:  Sessions
---

{% comment %}
        The code below dynamically generates a sidebar nav of pages with
        `layout: page` in the front-matter. See readme for usage.
{% endcomment %}

{% for page in site.pages %}
{% if page.session == true %}
<entry>
   <a href="{{ page.url }}"/>{{ page.title }}</a>
 </entry>
{% endif %}
{% endfor %}

http://stackoverflow.com/questions/17118551/generating-a-list-of-pages-not-posts-in-a-given-category