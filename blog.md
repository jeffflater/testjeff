---
layout: post-sidebar
title: "Blog"
hero_image: /assets/img/testjeff-web-logo-min.png
hero_alt: Latest from the blog
---

<ul class="post-list">
  {% assign posts_sorted = paginator.posts | default: site.posts | sort: "date" | reverse %}
  {% for p in posts_sorted %}
  <li class="post-list-item">
    <h2 class="h2"><a href="{{ p.url | relative_url }}">{{ p.title }}</a></h2>

    <p class="post-list-meta">
      <time datetime="{{ p.date | date_to_xmlschema }}">{{ p.date | date: "%b %-d, %Y" }}</time>
      {% if p.tags and p.tags.size > 0 %} • {{ p.tags | array_to_sentence_string }}{% endif %}
    </p>

    {% if p.excerpt %}
      <p>{{ p.excerpt | strip_html | truncate: 180 }}</p>
    {% endif %}
  </li>
  {% endfor %}
</ul>

{% if paginator %}
<nav class="pager">
  {% if paginator.previous_page %}
    <a href="{{ paginator.previous_page_path | relative_url }}">← Newer</a>
  {% endif %}
  {% if paginator.next_page %}
    <a href="{{ paginator.next_page_path | relative_url }}" style="float:right">Older →</a>
  {% endif %}
</nav>
{% endif %}
