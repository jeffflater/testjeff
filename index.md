---
layout: default
title: Learn API Test Automation with Jeff Flater
---

<!-- Hero Section -->
<section class="hero">
  <div class="container">
    <div class="hero__content">
      <h1 class="hero__title">Master API Test Automation with Modern Tools</h1>
      <p class="hero__subtitle">Learn Python, Behave, GitHub Copilot, and AI-powered testing from an instructor with 20+ years of experience. Build real-world automation frameworks you can use immediately.</p>
      <div class="hero__cta">
        <a href="https://www.udemy.com/course/testjeff-api-testing-using-python-behave-vs-code-github-copilot/?referralCode=A9712B7048F3109836AF" class="btn btn--udemy btn--large" target="_blank" rel="noopener">
          Explore My Courses
        </a>
        <a href="{{ '/about' | relative_url }}" class="btn btn--secondary btn--large">
          About Jeff
        </a>
      </div>
    </div>
  </div>
</section>

<!-- Featured Course Section -->
<section class="section">
  <div class="container">
    <div class="featured-course">
      <div class="featured-course__grid">
        <img src="{{ '/assets/img/testjeff-web-logo-min.png' | relative_url }}" alt="API Testing Course" class="featured-course__image">

        <div class="featured-course__content">
          <div class="featured-course__badge">
            <span class="badge">Bestseller</span>
          </div>

          <h2 class="featured-course__title">API Testing with Python, Behave, VS Code & GitHub Copilot</h2>

          <p class="featured-course__desc">
            A modern, AI-powered approach to API testing. Learn to test REST, SOAP, GraphQL, WebSocket, and Blockchain APIs. Build complete automation frameworks with BDD, Python, and GitHub Actions.
          </p>

          <div class="featured-course__stats">
            <div class="stat">
              <div class="stat__value">5+ hours</div>
              <div class="stat__label">On-demand video</div>
            </div>
            <div class="stat">
              <div class="stat__value">6 projects</div>
              <div class="stat__label">Hands-on labs</div>
            </div>
            <div class="stat">
              <div class="stat__value">Lifetime</div>
              <div class="stat__label">Access</div>
            </div>
          </div>

          <a href="https://www.udemy.com/course/testjeff-api-testing-using-python-behave-vs-code-github-copilot/?referralCode=A9712B7048F3109836AF" class="btn btn--udemy btn--large" target="_blank" rel="noopener">
            Enroll Now on Udemy
          </a>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- What You'll Learn Section -->
<section class="section" style="background: var(--bg-secondary);">
  <div class="container">
    <div class="section__header">
      <h2 class="section__title">What You'll Learn</h2>
      <p class="section__subtitle">Skills you'll gain from this course</p>
    </div>

    <div class="course-grid">
      <div class="course-card">
        <div style="padding: 24px; background: var(--bg-primary); height: 100%;">
          <div style="font-size: 3rem; margin-bottom: 16px;">🐍</div>
          <h3 class="course-card__title">Python & Behave</h3>
          <p style="color: var(--text-secondary); font-size: 0.875rem;">Write clean BDD scenarios with Gherkin syntax and Python step definitions</p>
        </div>
      </div>

      <div class="course-card">
        <div style="padding: 24px; background: var(--bg-primary); height: 100%;">
          <div style="font-size: 3rem; margin-bottom: 16px;">🤖</div>
          <h3 class="course-card__title">AI-Powered Testing</h3>
          <p style="color: var(--text-secondary); font-size: 0.875rem;">Use GitHub Copilot to generate smarter tests faster and boost productivity</p>
        </div>
      </div>

      <div class="course-card">
        <div style="padding: 24px; background: var(--bg-primary); height: 100%;">
          <div style="font-size: 3rem; margin-bottom: 16px;">🔌</div>
          <h3 class="course-card__title">API Protocols</h3>
          <p style="color: var(--text-secondary); font-size: 0.875rem;">Test REST, SOAP, GraphQL, WebSocket, and Blockchain APIs</p>
        </div>
      </div>

      <div class="course-card">
        <div style="padding: 24px; background: var(--bg-primary); height: 100%;">
          <div style="font-size: 3rem; margin-bottom: 16px;">⚙️</div>
          <h3 class="course-card__title">CI/CD Pipelines</h3>
          <p style="color: var(--text-secondary); font-size: 0.875rem;">Automate testing with GitHub Actions and Docker containers</p>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- Instructor Section -->
<section class="section">
  <div class="container">
    <div class="section__header">
      <h2 class="section__title">Meet Your Instructor</h2>
    </div>

    <div style="display: grid; grid-template-columns: 200px 1fr; gap: 32px; align-items: start;">
      <img src="{{ '/assets/img/testjeff-web-logo-min.png' | relative_url }}" alt="Jeff Flater" style="border-radius: 50%; width: 200px; height: 200px; object-fit: cover; border: 4px solid var(--udemy-purple);">

      <div>
        <h3 style="font-size: 1.5rem; margin-bottom: 8px;">Jeff Flater</h3>
        <p style="color: var(--text-secondary); margin-bottom: 16px;">Test Automation Expert • Course Creator • Open Source Contributor</p>

        <p style="margin-bottom: 16px;">
          I've spent 20+ years in software — the first 10 in development and the last 10 focused on test automation, CI/CD pipelines, and modern testing frameworks. This unique perspective helps me teach testing from both sides.
        </p>

        <p style="margin-bottom: 24px;">
          Through TestJeff, I create practical, hands-on courses that help software testers and QA engineers level up their automation skills with modern tools like Python, Behave, GitHub Copilot, and AI-powered testing.
        </p>

        <a href="{{ '/about' | relative_url }}" class="btn btn--secondary">
          Learn More About Jeff
        </a>
      </div>
    </div>
  </div>
</section>

<!-- Latest Blog Posts -->
<section class="section" style="background: var(--bg-secondary);">
  <div class="container">
    <div class="section__header">
      <h2 class="section__title">Latest from the Blog</h2>
      <p class="section__subtitle">Tips, tutorials, and insights on test automation</p>
    </div>

    {% for post in site.posts limit:3 %}
    <div style="background: var(--bg-primary); border: 1px solid var(--border-light); border-radius: var(--radius); padding: 24px; margin-bottom: 16px;">
      <h3 style="font-size: 1.25rem; margin-bottom: 8px;">
        <a href="{{ post.url | relative_url }}" style="color: var(--text-primary);">{{ post.title }}</a>
      </h3>
      <p style="color: var(--text-muted); font-size: 0.875rem; margin-bottom: 12px;">{{ post.date | date: "%B %-d, %Y" }}</p>
      {% if post.excerpt %}
        <p style="color: var(--text-secondary);">{{ post.excerpt | strip_html | truncate: 200 }}</p>
      {% endif %}
    </div>
    {% endfor %}

    <a href="{{ '/blog' | relative_url }}" class="btn btn--secondary">View All Posts</a>
  </div>
</section>
