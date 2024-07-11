---
layout: default
title: Blog
---

{% for post in site.posts %}
<article>
  <h1><a href="{{ post.url }}">{{ post.title }}</a></h1>
  <div class="entry">
    {{ post.excerpt }}
  </div>
  <a href="{{ site.baseurl }}{{ post.url }}" class="read-more">Read More</a>
</article>
{% endfor %}
