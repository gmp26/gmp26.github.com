---
layout: page
title: Grumplet
tagline: experiments
---
{% include JB/setup %}

Refer to [Jekyll Quick Start](http://jekyllbootstrap.com/usage/jekyll-quick-start.html) or complete documentation at: [Jekyll Bootstrap](http://jekyllbootstrap.com)
    
## Posts
<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>




