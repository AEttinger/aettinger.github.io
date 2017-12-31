---

---
<main role="main" class="container">

<div class="row">

  <div class="col-sm-8 blog-main">

  {% for post in site.posts %}

    <div class="blog-post">
      <h2 class="blog-post-title">{{ post.title }}</h2>
      <p class="blog-post-meta">{{ post.date | date: "%B %d, %Y %k:%M %z" }}</p>
      {{ post.content }}
    </div>

  {% endfor %}

  </div>

</div>

</main>
