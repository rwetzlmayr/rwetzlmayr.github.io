---
layout: default
---

[Robert Wetzlmayr](https://wetzlmayr.at/) is a software developer and contributor to the open-source community.

He is best known for his contributions to the [Textpattern CMS](https://textpattern.com/about/contributors#core-team "The small content management system that can handle big ideas") project. He has worked on various aspects of the Textpattern project, including developing new features, fixing bugs, and improving performance.

In addition to his software development work, Wetzlmayr has a passion for photography and regularly shares his photos.

## Most recent posts

<div class="posts">
  {% for post in site.posts %}
    <article class="post">

      <h3><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h3>

      <div class="entry">
        {{ post.excerpt }}
      </div>

      <a href="{{ site.baseurl }}{{ post.url }}" class="read-more">Read on&hellip;</a>
    </article>
{% endfor %}
</div>



