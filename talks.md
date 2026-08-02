---
layout: default
title: Conference Talks
permalink: /talks/
---
<h1 class="page-title">Conference Talks</h1>
<p class="page-subtitle">Slides, video, and supplemental downloads for each talk. Talks are markdown files in <code>_talks/</code>.</p>

{% assign sorted_talks = site.talks | sort: "date" | reverse %}
{% if sorted_talks.size > 0 %}
<ul class="entry-list">
  {% for talk in sorted_talks %}
  <li>
    <div class="entry-meta">
      {{ talk.date | date: "%B %-d, %Y" }}
      {% if talk.event %}&middot; {{ talk.event }}{% endif %}
    </div>
    <h3><a href="{{ talk.url | relative_url }}">{{ talk.title }}</a></h3>
    <p>{{ talk.excerpt | strip_html | truncatewords: 30 }}</p>
  </li>
  {% endfor %}
</ul>
{% else %}
<p class="empty-state">No talks yet.</p>
{% endif %}
