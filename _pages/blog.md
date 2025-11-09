---
layout: page
title: Blog
permalink: /blog/
---

Work in progress!

<h2>Posts</h2>
<ul>
  {% for post in site.posts %}
    <li>
      <h3>
        <a href="{{ post.url }}">{{ post.title }}</a>
      </h3>
      {{ post.content | strip_html | truncatewords: 30}}
    </li>
  {% endfor %}
</ul>