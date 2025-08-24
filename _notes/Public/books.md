---
title: books
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
- dev - maybe for good books? 
[home](/benicerxd.github.io/README.md)