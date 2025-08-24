---
layout: sidebar
title: "Blog"
permalink: /blog/
hero_image: /assets/img/testjeff-web-logo-min.png
hero_alt: Latest from the blog
---

{% assign posts_list = paginator.posts | default: site.posts %}

{% if posts_list and posts_list.size > 0 %}
<ul class="post-list">
  {% for p in posts_list %}
  <li class="post-list-item" style="margin:1rem 0;">
    <a class="post-list-link" href="{{ p.url | relative_url }}">{{ p.title }}</a>
    <span class="post-date" style="color:#6b7280; margin-left:.5rem;">
      <time datetime="{{ p.date | date_to_xmlschema }}">{{ p.date | date: "%b %-d, %Y" }}</time>
    </span>

    {% if p.tags and p.tags.size > 0 %}
      <span class="post-tags" style="margin-left:.5rem;">• {{ p.tags | array_to_sentence_string }}</span>
    {% endif %}

    {% if p.excerpt %}
      <p class="post-excerpt">{{ p.excerpt | strip_html | truncate: 180 }}</p>
    {% endif %}
  </li>
  {% endfor %}
</ul>
{% else %}
<p>No posts yet. 🚧 Check back soon!</p>
{% endif %}

{% if paginator %}
<nav class="pager" aria-label="Pagination" style="display:flex;justify-content:space-between;margin-top:1.5rem;">
  <div>
    {% if paginator.previous_page %}
      <a rel="prev" href="{{ paginator.previous_page_path | relative_url }}">← Newer</a>
    {% endif %}
  </div>
  <div>
    {% if paginator.next_page %}
      <a rel="next" href="{{ paginator.next_page_path | relative_url }}">Older →</a>
    {% endif %}
  </div>
</nav>
{% endif %}
