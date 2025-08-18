---
layout: default
title: Home
---

# Supercharge Your API Test Automation
I’m **Jeff Flater**. Learn Python + Behave, VS Code, and AI with GitHub Copilot—fast.  
Finish a real test project in a single weekend.

## Quick Links
<div class="links-grid">
  <a class="link-card" href="{{ '/community' | relative_url }}">
    <div class="icon">🤝</div>
    <p class="link-title">Join the Test Automation CoP</p>
    <p class="link-sub">Community of Practice — free while we grow</p>
  </a>
  <a class="link-card" href="{{ '/courses' | relative_url }}">
    <div class="icon">📚</div>
    <p class="link-title">Courses</p>
    <p class="link-sub">Start with the API Testing course</p>
  </a>
  <a class="link-card" href="https://github.com/jeffflater" target="_blank" rel="noopener">
    <div class="icon">💻</div>
    <p class="link-title">GitHub: TestJeff</p>
    <p class="link-sub">Repos, examples, releases</p>
  </a>
  <a class="link-card" href="{{ '/about' | relative_url }}">
    <div class="icon">🙋‍♂️</div>
    <p class="link-title">About Jeff</p>
    <p class="link-sub">Who I am and how I teach</p>
  </a>
</div>

## Latest from the Blog
{% for post in site.posts limit:3 %}
<div class="post-item">
  <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
  <div class="post-date">{{ post.date | date: "%B %d, %Y" }}</div>
  {% if post.excerpt %}<div>{{ post.excerpt | strip_html | truncate: 140 }}</div>{% endif %}
</div>
{% endfor %}
<p><a href="{{ '/blog' | relative_url }}">View all posts →</a></p>
