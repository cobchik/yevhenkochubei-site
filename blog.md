---
layout: default
title: Блог
permalink: /blog/
---

<section class="hero">
  <h1>Блог</h1>
  <p class="lede">Статті про кризу сенсу, тривогу, стосунки та життя у нестабільний час.</p>
</section>

<section class="section">
  <ul class="post-list">
    {% for post in site.posts %}
    <li>
      <div class="post-title"><a href="{{ post.url | relative_url }}">{{ post.title }}</a></div>
      <div class="post-excerpt">{{ post.excerpt | strip_html | truncatewords: 28 }}</div>
    </li>
    {% endfor %}
  </ul>
</section>
