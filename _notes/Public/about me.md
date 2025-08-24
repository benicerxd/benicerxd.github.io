---
title: about me
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
[current books](/benicerxd.github.io/books.md)
[current webisites](/benicerxd.github.io/websites.md)
[current apps](/benicerxd.github.io/apps.md)
[current projects](/benicerxd.github.io/projects/)
[current notes](/benicerxd.github.io/notes/)

[home](/benicerxd.github.io/README.md)