---
title: Just. Image. It.
description: A blog about microscopy, microscope hardware, image processing, and sometimes biology.
---

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>

{% for post in site.posts limit: 10  %}
  {{ post.content }}
{% endfor %}
