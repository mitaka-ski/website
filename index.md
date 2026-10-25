---
layout: page
title: ホーム
permalink: /
---

三鷹市スキー連盟（Ski Association of Mitaka）の公式サイトです。

ご連絡は [mitaka_ski@yahoo.co.jp](mailto:mitaka_ski@yahoo.co.jp) までお願いいたします。

## 直近のお知らせ

{% assign recent = site.posts | slice: 0, 5 %}
{% if recent.size == 0 %}
現在、表示するお知らせはありません。
{% else %}
<ul>
  {% for post in recent %}
  <li>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    <span> — {{ post.date | date: "%Y-%m-%d" }}</span>
  </li>
  {% endfor %}
</ul>
{% endif %}
