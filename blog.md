---
layout: default
title: "Blog"
permalink: /blog/
---

<section class="hero">
  <div class="container">
    <div class="hero__content">
      <h1 class="hero__title">Latest from the Blog</h1>
      <p class="hero__subtitle">Insights on API testing, automation, AI-powered testing, and software quality</p>
    </div>
  </div>
</section>

<section class="section">
  <div class="container">
    <div style="max-width: 900px; margin: 0 auto;">
      {% assign posts_list = paginator.posts | default: site.posts %}

      {% if posts_list and posts_list.size > 0 %}
        <div style="display: grid; gap: 32px;">
          {% for post in posts_list %}
          <article style="padding: 32px; background: var(--bg-primary); border: 1px solid var(--border-light); border-radius: var(--radius); transition: box-shadow 0.2s ease, transform 0.2s ease;">
            <a href="{{ post.url | relative_url }}" style="text-decoration: none; color: inherit;">
              <h2 style="font-size: 1.75rem; margin-bottom: 12px; color: var(--text-primary);">{{ post.title }}</h2>

              <div style="display: flex; gap: 12px; align-items: center; margin-bottom: 16px; color: var(--text-secondary); font-size: 0.875rem;">
                <time datetime="{{ post.date | date_to_xmlschema }}">
                  {{ post.date | date: "%B %-d, %Y" }}
                </time>
                {% if post.tags and post.tags.size > 0 %}
                  <span>•</span>
                  <span>{{ post.tags | array_to_sentence_string }}</span>
                {% endif %}
              </div>

              {% if post.excerpt %}
                <p style="line-height: 1.7; color: var(--text-secondary); margin-bottom: 16px;">
                  {{ post.excerpt | strip_html | truncate: 240 }}
                </p>
              {% endif %}

              <span class="btn btn--secondary" style="display: inline-block; margin-top: 8px;">
                Read More →
              </span>
            </a>
          </article>
          {% endfor %}
        </div>

        {% if paginator %}
        <nav style="display: flex; justify-content: space-between; margin-top: 48px; padding-top: 32px; border-top: 1px solid var(--border-light);">
          <div>
            {% if paginator.previous_page %}
              <a href="{{ paginator.previous_page_path | relative_url }}" class="btn btn--secondary">← Newer Posts</a>
            {% endif %}
          </div>
          <div>
            {% if paginator.next_page %}
              <a href="{{ paginator.next_page_path | relative_url }}" class="btn btn--secondary">Older Posts →</a>
            {% endif %}
          </div>
        </nav>
        {% endif %}

      {% else %}
        <div style="text-align: center; padding: 64px 24px; background: var(--bg-secondary); border-radius: var(--radius);">
          <div style="font-size: 4rem; margin-bottom: 16px;">📝</div>
          <h3 style="font-size: 1.5rem; margin-bottom: 8px;">No Posts Yet</h3>
          <p style="color: var(--text-secondary);">Check back soon for articles on API testing, automation, and modern testing practices!</p>
        </div>
      {% endif %}
    </div>
  </div>
</section>
