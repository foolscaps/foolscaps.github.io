---
layout: page
permalink: /blog/
title: blog
description: some articles I write for myself, some for others
---

<ul class="post-list">
    {% for post in site.posts %}
        {% if post.description %}
            <li>
                <h3><a class="post-title" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h3>
                <span class="post-list-description">{{ post.description }}</span> &nbsp; &nbsp; &nbsp;
                <span class="post-list-meta">{{ post.date | date: '%B %-d, %Y' }}</span>
                <p></p>
                <hr/>
            </li>
        {% endif %}
    {% endfor %}
</ul>
