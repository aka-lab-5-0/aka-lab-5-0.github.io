---
layout: default
title: 一般社団法人 赤ちゃんラボ5.0について
items:
  - url: about.html
    title: 赤ちゃんラボ5.0について
  - title: ニュース
  - url: join.html
    title: ご協力のお願い
---

# ニュース

{% for post in site.posts %}
- [{{ post.title }}]({{ post.url | relative_url }})
  {{ post.date | date: "%Y-%m-%d" }}
{% endfor %}
