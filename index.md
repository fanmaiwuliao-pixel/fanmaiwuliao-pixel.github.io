---
layout: default
title: 引得
---
# 引得

**你的名字（Your Name）**，〔在这里写一两句自我介绍：学历、现任职务、研究方向。例如：××大学历史学系博士，现任××大学××学院副教授，研究方向为……〕

---

**Curriculum vitae**　[学历](/cv/#学历)｜

**Blog**　[站内所有文章](/blog/)：如博客般依时间顺序从新到旧列出。

---

## 最新文章

- {% for post in site.posts limit: 5 %}
- {{ post.date | date: "%Y 年 %-m 月 %-d 日" }} [{{ post.title }}]({{ post.url | relative_url }})

  {{ post.excerpt | strip_html | truncate: 100 }}
-  {% endfor %}

