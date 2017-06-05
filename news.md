---
layout: post
title: news
permalink: /news/
---

<ul class="post-list">
    {% for post in paginator.posts %}
      <li>
        <h2><a class="post-title" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h2>
        <p class="post-meta">{{ post.date | date: '%B %-d, %Y — %H:%M' }}</p>
        <p>{{ post.description }}</p>
        <br/>
        <hr/>
      </li>
    {% endfor %}
</ul>


<ul>
  {% for post in site.posts %}
    <li>
      <a class="post-title" href="{{ post.url }}">{{ post.title }}</a>
      <br />
      {{ post.excerpt }}
    </li>
        <hr />
        <p>&nbsp;</p>
  {% endfor %}

</ul>
