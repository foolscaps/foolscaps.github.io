---
layout: page
permalink: /blog/
title: blog
description: Some articles I write for myself, some for others.
---

<ul class="post-list">
    {% for post in site.posts %}
      <li>
        <h3><a class="post-title" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h3>
        <p class="post-meta">{{ post.date | date: '%B %-d, %Y' }}</p>
        <p>{{ post.description }}</p>
        <br/>
        <hr/>
      </li>
    {% endfor %}
</ul>