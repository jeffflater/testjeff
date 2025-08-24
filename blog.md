---
layout: sidebar
title: Blog
hero_image: /assets/img/testjeff-web-logo-min.png
hero_alt: Latest from the blog
---

# Blog
<ul>
{% for post in site.posts %}
  <li>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    — <span class="post-date">{{ post.date | date: "%B %d, %Y" }}</span>
  </li>
{% endfor %}
</ul>
