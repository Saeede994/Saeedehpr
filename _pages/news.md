---
layout: archive
title: "News"
permalink: /news/
---

<h1>Latest News</h1>

<ul>
  {% for post in site.news %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a> - {{ post.date | date: "%B %d, %Y" }}
      <p>{{ post.description }}</p>
    </li>
  {% endfor %}
</ul>
