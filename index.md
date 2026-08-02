---
layout: default
title: Home
---
<section class="hero">
  <h1>Hi, I'm <span class="accent">{{ site.author.name }}</span>.</h1>
  <p>{{ site.description }}</p>
  <div class="social-links">
    <a href="https://github.com/{{ site.author.github }}">GitHub</a>
    {% if site.author.linkedin %}<a href="https://linkedin.com/in/{{ site.author.linkedin }}">LinkedIn</a>{% endif %}
    {% if site.author.twitter %}<a href="https://twitter.com/{{ site.author.twitter }}">Twitter</a>{% endif %}
  </div>
</section>

<div class="card-grid">
  <a class="card" href="https://anthonycastano.com/">
    <span class="card-icon">&#9998;</span>
    <h3>Blog</h3>
    <p>Writing on things I'm building and learning.</p>
  </a>
  <a class="card" href="{{ '/talks/' | relative_url }}">
    <span class="card-icon">&#127908;</span>
    <h3>Conference Talks</h3>
    <p>Slides, videos, and supplemental downloads from talks I've given.</p>
  </a>
  <a class="card" href="{{ '/projects/' | relative_url }}">
    <span class="card-icon">&#9881;</span>
    <h3>Projects</h3>
    <p>Things I've built, open source and otherwise.</p>
  </a>
  <a class="card" href="https://anthonycastano.com/contact-me/">
    <span class="card-icon">&#9993;</span>
    <h3>Contact</h3>
    <p>Get in touch.</p>
  </a>
</div>
