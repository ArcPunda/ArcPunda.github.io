---
layout: default
title: "Home"
---

<div class="columns">
  <div class="column">
    <h2>Left Column</h2>
    <ul>
      <li><a href="#">Home</a></li>
      <li><a href="#">About</a></li>
      <li><a href="#">Projects</a></li>
      <li><a href="#">Blog</a></li>
      <li><a href="#">Contact</a></li>
    </ul>
  </div>

  <div class="column">
    <h1>Welcome to Glenn’s Tech Blog 👋</h1>
    <p>Hi, I’m Glenn — a fresh IT graduate exploring tech, coding, and data.</p>
    <p>Here I’ll share my <strong>projects, tutorials, and learnings</strong> as I grow in the IT field.</p>

    <h2>Latest Posts</h2>
    <ul>
      {% for post in site.posts %}
        <li><a href="{{ post.url | relative_url }}">{{ post.title }}</a></li>
      {% endfor %}
    </ul>
  </div>

  <div class="column">
    <h2>Right Column</h2>
    <p><strong>ArcticPunda &lt;Dev&gt; Blog</strong></p>
    <p>A fresh graduate’s journey in IT – projects, dumb stuff, and learning as an IT professional.</p>
  </div>
</div>
