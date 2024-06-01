---
layout: default
title: ニュース
items:
  - url: index.html
    title: トップページ
  - url: about.html
    title: 赤ちゃんラボ5.0について
  - title: ニュース
  - url: activity.html
    title: 活動情報/資料
    class: detail
  - url: join.html
    title: ご協力のお願い
  - url: faq.html
    title: FAQ(よくあるご質問)
    class: detail
  - url: contact.html
    title: お問い合わせ
---

# ニュース

{% for post in site.posts %}
- [{{ post.title }}]({{ post.url | relative_url }})
  {{ post.date | date: "%Y-%m-%d" }}
{% endfor %}
