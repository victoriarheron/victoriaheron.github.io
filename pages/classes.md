---
layout: page
show_meta: false
subheadline: "Come practice with me"
header: no
image:
    title: "practice_with_me.jpg"
    caption:
    caption_url:
permalink: "/classes/"
---

<h5>
My <a href="{{site.url}}/classes/schedule">schedule</a> changes often but I always try to make room for private lessons:
</h5>
<ul>
    {% for post in site.categories.classes %}
    <li><a href="{{ site.url }}{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
</ul>