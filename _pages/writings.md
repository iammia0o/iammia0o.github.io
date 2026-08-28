---
layout: page
permalink: /writings/
title: WRITINGS
description: Some of my reflection about life :) 
description_italic: false
nav: true
nav_order: 4
---

<div class="writings">
  <div class="grid">
    <div class="grid-sizer"></div>
    {% assign writings = site.writings | sort: "date" | reverse %}
    {% for post in writings %}
    <div class="grid-item">
      <a href="{{ post.url | relative_url }}">
        <div class="card hoverable">
          {% if post.img %}
          {% include figure.html path=post.img alt=post.title %}
          {% endif %}
          <div class="card-body">
            <h2 class="card-title">{{ post.title }}</h2>
            <p class="card-text font-italic">{{ post.description }}</p>
            <p class="card-text text-muted small mb-0">{{ post.date | date: "%b %-d, %Y" }}</p>
          </div>
        </div>
      </a>
    </div>
    {% endfor %}
  </div>
</div>
