---

---
{% include navbar.html %}

{% for post in site.posts limit: 10  %}
  {{ post.content }}
{% endfor %}

{% include footer.html %}
