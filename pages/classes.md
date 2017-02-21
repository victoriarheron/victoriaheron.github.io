---
layout: page
show_meta: false
title: "Schedule or attend a class!"
subheadline: "My schedule changes often but I always try to make room in my schedule for private lessons"
header:
   image_fullwidth: "header_unsplash_5.jpg"
permalink: "/classes/"
---
<ul>
    {% for post in site.categories.classes %}
    <li><a href="{{ site.url }}{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
</ul>