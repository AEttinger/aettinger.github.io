---

---
<main role="main" class="container">

<div class="row">

  <div class="col-sm-8 blog-main">

  {% for post in paginator.posts %}

    <div class="blog-post">
      <h2 class="blog-post-title">{{ post.title }}</h2>
      <p class="blog-post-meta">{{ post.date | date: "%B %d, %Y %k:%M %Z" }}</p>
      {{ post.content }}
    </div>

  {% endfor %}

  </div>

  <nav class="blog-pagination">
    <a class="btn btn-outline-secondary disabled" href="{{ paginator.previous_page_path }}">Newer</a>
    {% if paginator.next_page %}
    <a class="btn btn-outline-primary" href="{{ paginator.next_page_path }}">Older</a>
    {% endif %}
  </nav>

</div>

</main>
