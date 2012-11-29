---
layout: page
title: Hello World!
tagline: Supporting tagline
---
{% include JB/setup %}

<div class="container">
  {% for post in site.posts %}
    <div class="span8">
      <h1>{{ post.title }}</h1>
      <p>{{ post.date | date_to_string }}</p>
      <p>{{ post.content }}</p>
    </div>
  {% endfor %}
</div>