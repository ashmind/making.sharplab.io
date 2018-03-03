---
title: Index
layout: index
---

{% for post in site.posts %}   
  <article class="post">
    <a name="{{post.id | remove_first: '/'}}" class="post-anchor"></a>
    <h2>{{post.title}}</h2>
    {{post.content}}
  </article>
{% endfor %}