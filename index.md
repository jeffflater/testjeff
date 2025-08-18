---
layout: sidebar
title: Supercharge Your API Test Automation
hero_image: /assets/img/testjeff-web-logo-min.png
hero_alt: testJeff brand
---

# Supercharge Your API Test Automation
I’m **Jeff Flater** — here to help you level up fast with **Python, Behave, VS Code, and AI with GitHub Copilot**.  
⚡ Build confidence, ship smarter tests, and finish a real-world project in just a **single weekend**.

---

## Quick Links
<div class="links-grid">
  <a class="link-card" href="{{ '/community' | relative_url }}">
    <div class="icon">🤝</div>
    <div class="link-title">Join the Test Automation CoP</div>
    <p class="link-sub">Community of Practice — free while we grow</p>
  </a>

  <a class="link-card" href="{{ '/courses' | relative_url }}">
    <div class="icon">📚</div>
    <div class="link-title">Courses</div>
    <p class="link-sub">Start with the API Testing course</p>
  </a>

  <a class="link-card" href="{{ '/github' | relative_url }}">
    <div class="icon">💻</div>
    <div class="link-title">GitHub</div>
    <p class="link-sub">Repos, examples, and course code</p>
  </a>

  <a class="link-card" href="{{ '/about' | relative_url }}">
    <div class="icon">🙋‍♂️</div>
    <div class="link-title">About Jeff</div>
    <p class="link-sub">Who I am and how I teach</p>
  </a>
</div>

---

## Latest from the Blog
{% for post in site.posts limit:3 %}
<div class="post-item">
  <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
  <div class="post-date">{{ post.date | date: "%B %-d, %Y" }}</div>
  {% if post.excerpt %}
    <p>{{ post.excerpt | strip_html | truncate: 140 }}</p>
  {% endif %}
</div>
{% endfor %}
<p><a href="{{ '/blog' | relative_url }}">View all posts →</a></p>
