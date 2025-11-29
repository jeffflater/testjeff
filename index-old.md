---
layout: sidebar
title: API Test Automation Courses by Jeff Flater
hero_image: /assets/img/testjeff-web-logo-min.png
hero_alt: testJeff brand
---

# Hey, I'm Jeff Flater 👋

I teach **software testers and QA engineers** how to master **API test automation** with modern tools like Python, Behave, GitHub Copilot, and AI-powered testing.

**20+ years in software** (10 in dev, 10 in testing) • Creator of courses trusted by thousands • Open-source contributor

---

## 🎓 Featured Course

<div class="course-hero">
  <div class="course-hero__badge">
    <span class="badge">NEW COURSE</span>
  </div>
  <h3 class="course-hero__title">API Testing with Python, Behave, VS Code & GitHub Copilot</h3>
  <p class="course-hero__desc">
    A modern, AI-powered approach to API testing. Learn to test REST, SOAP, GraphQL, WebSocket, and Blockchain APIs in a single weekend. Build real automation frameworks with BDD, Python, and GitHub Actions.
  </p>

  <div class="course-hero__stats">
    <div class="stat">
      <div class="stat__value">5+ hours</div>
      <div class="stat__label">Video content</div>
    </div>
    <div class="stat">
      <div class="stat__value">6 projects</div>
      <div class="stat__label">Hands-on labs</div>
    </div>
    <div class="stat">
      <div class="stat__value">100%</div>
      <div class="stat__label">Practical</div>
    </div>
  </div>

  <a href="https://www.udemy.com/course/testjeff-api-testing-using-python-behave-vs-code-github-copilot/?referralCode=A9712B7048F3109836AF" class="btn btn--primary" target="_blank" rel="noopener">
    Enroll on Udemy →
  </a>
</div>

---

## 🚀 What You'll Learn

<div class="skills-grid">
  <div class="skill-item">
    <div class="skill-icon">🐍</div>
    <div class="skill-name">Python & Behave</div>
    <div class="skill-desc">Write clean BDD scenarios with Gherkin syntax</div>
  </div>

  <div class="skill-item">
    <div class="skill-icon">🤖</div>
    <div class="skill-name">AI-Powered Testing</div>
    <div class="skill-desc">Use GitHub Copilot to generate smarter tests faster</div>
  </div>

  <div class="skill-item">
    <div class="skill-icon">🔌</div>
    <div class="skill-name">API Protocols</div>
    <div class="skill-desc">REST, SOAP, GraphQL, WebSocket, Blockchain APIs</div>
  </div>

  <div class="skill-item">
    <div class="skill-icon">⚙️</div>
    <div class="skill-name">CI/CD Pipelines</div>
    <div class="skill-desc">Automate with GitHub Actions & Docker</div>
  </div>
</div>

---

## 💬 What Students Say

<div class="testimonial">
  <p class="testimonial__quote">"Jeff's approach to teaching API testing is refreshingly practical. No fluff, just real-world skills you can use immediately."</p>
  <div class="testimonial__author">— Course Student</div>
</div>

---

## 📚 More Coming Soon

I'm actively creating new courses on:
- **Java with Cucumber** for API testing
- **TypeScript with Cucumber** for modern test automation
- **Performance testing** with modern tools
- **Advanced CI/CD** for test architects

Want to be notified? Follow me on [GitHub](https://github.com/jeffflater) or check the [blog](/blog) for updates.

---

## 📝 Latest from the Blog

{% for post in site.posts limit:3 %}
<div class="post-item">
  <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
  <div class="post-date">{{ post.date | date: "%B %-d, %Y" }}</div>
  {% if post.excerpt %}
    <p>{{ post.excerpt | strip_html | truncate: 140 }}</p>
  {% endif %}
</div>
{% endfor %}

<a href="{{ '/blog' | relative_url }}" class="btn btn--secondary">View all posts →</a>
