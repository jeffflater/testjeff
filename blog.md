---
layout: sidebar
title: "Blog"
permalink: /blog/
hero_image: /assets/img/testjeff-web-logo-min.png
hero_alt: Latest from the blog
---

# 📝 Latest from the Blog

{% assign posts_list = paginator.posts | default: site.posts %}

{% if posts_list and posts_list.size > 0 %}
  {% for post in posts_list %}
  <div class="post-item">
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    <div class="post-date">
      <time datetime="{{ post.date | date_to_xmlschema }}">
        {{ post.date | date: "%B %-d, %Y" }}
      </time>
      {% if post.tags and post.tags.size > 0 %}
        • {{ post.tags | array_to_sentence_string }}
      {% endif %}
    </div>
    {% if post.excerpt %}
      <p>{{ post.excerpt | strip_html | truncate: 180 }}</p>
    {% endif %}
  </div>
  {% endfor %}
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
