---
layout: default
title: 所有文章
permalink: /blog/
---

# 所有文章

<ul class="post-list">
{% for post in site.posts %}
  <li>
    <span class="date">{{ post.date | date: "%Y 年 %-m 月 %-d 日" }}</span>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
  </li>
{% endfor %}
</ul>
