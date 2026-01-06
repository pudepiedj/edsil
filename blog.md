---
layout: default
title: Blog
permalink: /blog/
---
<section class="hero">
  <div class="container">
    <div class="hero-content">
      <p class="hero-tagline">Blog</p>
      <h1>Thoughts on <span class="highlight">Education and Leadership</span></h1>
      <p class="hero-lead">
        Reflections from decades of founding and leading international schools.
      </p>
    </div>
  </div>
</section>

<section>
  <div class="container">
    {% for post in site.posts %}
    <article style="margin-bottom: 2em; padding-bottom: 1.5em; border-bottom: 1px solid rgba(255,255,255,0.1);">
      <h3 style="margin-bottom: 0.3em;">
        <a href="{{ post.url | relative_url }}" style="text-decoration: none; color: inherit;">{{ post.title }}</a>
      </h3>
      <p style="color: rgba(255,255,255,0.6); font-size: 0.9em; margin-bottom: 0.8em;">
        {{ post.date | date: "%B %-d, %Y" }}{% if post.author %} &bull; {{ post.author }}{% endif %}
      </p>
      <div style="line-height: 1.6;">
        {{ post.excerpt }}
      </div>
    </article>
    {% endfor %}
    
    {% if site.posts.size == 0 %}
    <p>No posts yet. Check back soon!</p>
    {% endif %}
  </div>
</section>
