---
layout: page
show_meta: false
subheadline: "My schedule changes often but I always try to make room in my schedule for private lessons"
header: no
image:
    title: "bodyonyoga.png"
    caption: caption words
    caption_url: www.google.com
permalink: "/classes/"
---

<h2>
Come practice with me
</h2> 
<ul>
    {% for post in site.categories.classes %}
    <li><a href="{{ site.url }}{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
</ul>