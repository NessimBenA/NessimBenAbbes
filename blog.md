---
layout: page
title: Blog
permalink: /blog/
---

{% if site.posts.size > 0 %}
  <ul>
    {% for post in site.posts %}
      <li>
        <h3><a href="{{ post.url | relative_url }}">{{ post.title | escape }}</a></h3>
        <p>{{ post.date | date: "%B %d, %Y" }}</p>
        <p>{{ post.excerpt }}</p>
      </li>
    {% endfor %}
  </ul>
{% else %}
  <p>No posts yet. Check back soon!</p>
{% endif %}
