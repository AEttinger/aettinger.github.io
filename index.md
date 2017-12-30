---

---
{% include navbar.html %}

<div class="row">

  <div class="col-sm-8 blog-main">

{% for post in site.posts limit: 10  %}
  {{ post.content }}
{% endfor %}

  </div>
</div>

{% include footer.html %}
