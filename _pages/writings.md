---
layout: page
permalink: /writings/
title: WRITINGS
description: Some of my reflection about life :) 
description_italic: false
nav: true
nav_order: 4
---

{% assign series_list = site.series | sort: "date" | reverse %}
{% assign standalone = site.writings | where_exp: "w", "w.series == nil" | sort: "date" | reverse %}

<div class="writings">
  <div class="grid">
    <div class="grid-sizer"></div>

    {% for s in series_list %}
    {% assign parts = site.writings | where: "series", s.slug %}
    <div class="grid-item">
      <a href="{{ s.url | relative_url }}">
        <div class="card hoverable series-card">
          <span class="series-card-badge">{{ parts | size }} parts</span>
          {% if s.img %}
          {% include figure.html path=s.img alt=s.title %}
          {% endif %}
          <div class="card-body">
            <h2 class="card-title">{{ s.title }}</h2>
            <p class="card-text font-italic">{{ s.description }}</p>
            <p class="card-text text-muted small mb-0">A series</p>
          </div>
        </div>
      </a>
    </div>
    {% endfor %}

    {% for post in standalone %}
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
