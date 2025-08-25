---
title: f1 powerbi dashboard
feed: show
date: 2024-01-15
tags:
  - "#projects/future"
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
- will start this one day 
[home](/benicerxd.github.io/README.md) 