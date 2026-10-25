---
layout: page
title: ホーム
permalink: /
---

三鷹市スキー連盟（Ski Association of Mitaka）は、三鷹市体育協会の公認スキークラブです。  
ウィンターシーズンにスキーツアーやバッジテストを実施し、初めての方からエキスパートまで楽しめる活動を行っています。

ご連絡は [mitaka_ski@yahoo.co.jp](mailto:mitaka_ski@yahoo.co.jp) までお願いいたします。

- [クラブ紹介]({{ "/about/" | relative_url }})
- [行事予定]({{ "/events/" | relative_url }})
- [会員募集]({{ "/join/" | relative_url }})
- [スキーツアーの様子]({{ "/skitour/" | relative_url }})

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
