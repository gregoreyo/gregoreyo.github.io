---
layout: default
title: Blog
permalink: /blog/
---
<h1 class="page-title">Blog</h1>
<p class="page-subtitle">Posts are plain markdown files in <code>_posts/</code>.</p>

{% if site.posts.size > 0 %}
<ul class="entry-list">
  {% for post in site.posts %}
  <li>
    <div class="entry-meta">
      {{ post.date | date: "%B %-d, %Y" }}
      {% for tag in post.tags %}<span class="tag">{{ tag }}</span>{% endfor %}
    </div>
    <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
    <p>{{ post.excerpt | strip_html | truncatewords: 30 }}</p>
  </li>
  {% endfor %}
</ul>
{% else %}
<p class="empty-state">No posts yet.</p>
{% endif %}
