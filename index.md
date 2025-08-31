---
layout: sidebar
title: Supercharge Your API Test Automation
hero_image: /assets/img/testjeff-web-logo-min.png
hero_alt: testJeff brand
---

# Supercharge Your Test Automation  
I’m **Jeff Flater** — creator of **TestJeff**.  
Here to help you level up fast with modern tools, smart workflows, and AI-powered testing.  
⚡ Build confidence, automate smarter, and finish real-world projects in record time.  

---

## Quick Links
<div class="links-grid">
  <a class="link-card" href="{{ '/community' | relative_url }}">
    <div class="icon">🤖</div>
    <div class="link-title">Discord</div>
    <p class="link-sub">Community of Practice — free and simple</p>
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
    <div class="link-title">About</div>
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
