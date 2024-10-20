---
layout: archive
title: "News"
permalink: /news/
---

<ul>
  {% for post in site.news %}
    <li>
      <strong>{{ post.title }}</strong> - {{ post.date | date: "%B %d, %Y" }}
      <p>{{ post.description }}</p>
    </li>
  {% endfor %}
</ul>
