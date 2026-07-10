---
layout: default
title: 引得
---
# 引得

**贩卖无聊（fanmaiwuliao）**，〔在这里写一两句自我介绍：〕

---

**Curriculum vitae**　[学历](/cv/#学历)｜

**Blog**　[站内所有文章](/blog/)：如博客般依时间顺序从新到旧列出。

---

## 最新文章

- {% for post in site.posts limit: 5 %}
- {{ post.date | date: "%Y 年 %-m 月 %-d 日" }} [{{ post.title }}]({{ post.url | relative_url }})

  {{ post.excerpt | strip_html | truncate: 100 }}
- {% endfor %}

