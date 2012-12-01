---
layout: page
title: Chiapei's Blog
tagline: Supporting tagline
---
{% include JB/setup %}

<div class="container">
  {% for post in site.posts %}
  <div class="span8">
    <div class="post_title">
      <h1><a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></h1>
    </div>
    <span class="label">{{ post.date | date_to_string }}</span>
    <p>{{ post.content }}</p>
    <p class="post_end">EOF</p>
  </div>
  {% endfor %}
</div>