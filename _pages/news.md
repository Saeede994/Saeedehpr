---
layout: archive
title: "News"
permalink: /news/
---

<ul>
  {% assign sorted_news = site.news | sort: 'date' %}
  {% for post in sorted_news %}
    <li>
      <strong>{{ post.title }}</strong> - {{ post.date | date: "%B %d, %Y" }}
      <p>{{ post.description }}</p>
    </li>
  {% endfor %}
</ul>