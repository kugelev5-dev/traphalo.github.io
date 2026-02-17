---
layout: page
title: Blog
permalink: /blog/
---

# Blog Posts

Welcome to my blog! Here you'll find posts about various topics I'm interested in.

{% for post in site.posts %}
  <article>
    <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
    <p class="post-meta">{{ post.date | date: "%B %-d, %Y" }}</p>
    <p>{{ post.excerpt }}</p>
  </article>
{% endfor %}
