---
layout: default
published: true
---

## Blog post archive

<div class="posts">
  {% for post in site.posts limit:42 %}
    <article class="post">

      <h3><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h3>

      <div class="entry">
        {{ post.excerpt }}
      </div>

      <a href="{{ site.baseurl }}{{ post.url }}" class="read-more">Read on&hellip;</a>
    </article>
{% endfor %}
</div>
