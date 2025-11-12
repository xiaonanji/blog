---
layout: base.html
permalink: /posts/
---

# Blog Posts

{% for post in collections.posts %}
  <article>
    <h2><a href="{{ post.url }}">{{ post.data.title }}</a></h2>
    <time>{{ post.date | dateFilter }}</time>
    <p>{{ post.data.excerpt }}</p>
  </article>
{% endfor %}
