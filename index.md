---
layout: default
---

## Hi this is my site

This is the **index** page.

This site is built with Jekyll.

<ul class="posts">
{% for post in site.posts limit: 20 %}
  <div class="post_info">
    <li>
         <a href="{{ post.url }}">{{ post.title }}</a> 
         <span>({{ post.date | date:"%Y-%m-%d" }})</span>
    </li>
    </div>
  {% endfor %}
</ul>
