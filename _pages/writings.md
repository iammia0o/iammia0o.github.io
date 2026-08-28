---
layout: page
permalink: /writings/
title: writings
description: Some of my reflection about life :) 
nav: true
nav_order: 4
---

<div class="post">
  <ul class="post-list">
    {% assign writings = site.writings | sort: "date" | reverse %}
    {% for post in writings %}
    {% assign read_time = post.content | number_of_words | divided_by: 180 | plus: 1 %}
    <li>
      <h3>
        <a class="post-title" href="{{ post.url | relative_url }}">{{ post.title }}</a>
      </h3>
      {% if post.description %}<p class="post-description">{{ post.description }}</p>{% endif %}
      <p class="post-meta">
        {{ post.date | date: "%B %-d, %Y" }} &nbsp;&middot;&nbsp; {{ read_time }} min read
      </p>
    </li>
    {% endfor %}
  </ul>
</div>
