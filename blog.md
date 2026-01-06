---
layout: default
title: Blog
permalink: /blog/
---
<section class="blog-list">
    <h1>Blog</h1>
    
    {% for post in site.posts %}
    <article>
        <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
        <p class="post-meta">{{ post.date | date: "%B %-d, %Y" }}{% if post.author %} &bull; {{ post.author }}{% endif %}</p>
        <div class="post-excerpt">
            {% if post.excerpt %}
                {{ post.excerpt }}
            {% endif %}
        </div>
    </article>
    {% endfor %}
    
    {% if site.posts.size == 0 %}
    <p>No posts yet. Check back soon!</p>
    {% endif %}
</section>
