---
layout: default
title: "Home"
---

<div class="columns">
  <!-- Left Column -->
  <div class="column left-col">
    <h2>Navigation</h2>
    <ul>
      <li><a href="{{ '/' | relative_url }}">Home</a></li>
      <li><a href="{{ '/about' | relative_url }}">About</a></li>
      <li><a href="{{ '/projects' | relative_url }}">Projects</a></li>
      <li><a href="{{ '/blog' | relative_url }}">Blog</a></li>
      <li><a href="{{ '/contact' | relative_url }}">Contact</a></li>
    </ul>
  </div>

  <!-- Middle Column -->
  <div class="column middle-col">
    <h1>Welcome to Glenn’s Tech Blog 👋</h1>
    <p>Hi, I’m Glenn — a fresh IT graduate exploring tech, coding, and data.<br>
    Here I’ll share my <strong>projects, tutorials, and learnings</strong> as I grow in the IT field.</p>

    <p>👉 Check out my latest posts below!</p>

    <h2>Latest Blog Posts</h2>
    <ul>
      {% for post in site.posts %}
        <li><a href="{{ post.url | relative_url }}">{{ post.title }}</a></li>
      {% endfor %}
    </ul>
  </div>

  <!-- Right Column -->
  <div class="column right-col">
    <h2>About This Blog</h2>
    <p><strong>ArcticPunda &lt;Dev&gt; Blog</strong></p>
    <p>A fresh graduate’s journey in IT – projects, tutorials, and learnings.</p>
  </div>
</div>
