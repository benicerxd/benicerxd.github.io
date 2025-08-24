---
title: websites
feed: show
date: 2024-01-15
tag:
  - "#personal"
---
```
{% for tag in site.tags %}
  <h3>{{ tag[0] }}</h3>
  <ul>
    {% for post in tag[1] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}
```
# cool websites
- [bible memorization](https://web.remem.me/) website (and app) that helps memorize verse for free 
- [text emojis](https://emojicombos.com/) search through text emojis ◝(ᵔᗜᵔ)◜, used mainly in coding headers
- [libby](https://libbyapp.com/) virtual library to read ebooks
[home](/benicerxd.github.io/README.md)