---
layout: default
title: Contact
permalink: /contact/
---
<h1 class="page-title">Contact</h1>
<p class="page-subtitle">The best ways to reach me.</p>

<div class="card-grid">
  <a class="card" href="mailto:{{ site.author.email }}">
    <span class="card-icon">&#9993;</span>
    <h3>Email</h3>
    <p>{{ site.author.email }}</p>
  </a>
  <a class="card" href="https://github.com/{{ site.author.github }}">
    <span class="card-icon">&#128187;</span>
    <h3>GitHub</h3>
    <p>@{{ site.author.github }}</p>
  </a>
  {% if site.author.linkedin %}
  <a class="card" href="https://linkedin.com/in/{{ site.author.linkedin }}">
    <span class="card-icon">&#128188;</span>
    <h3>LinkedIn</h3>
    <p>Let's connect.</p>
  </a>
  {% endif %}
  {% if site.author.twitter %}
  <a class="card" href="https://twitter.com/{{ site.author.twitter }}">
    <span class="card-icon">&#128226;</span>
    <h3>Twitter / X</h3>
    <p>@{{ site.author.twitter }}</p>
  </a>
  {% endif %}
</div>
