---
layout: single
title: Blog posts
---

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }} - {{ post.date  | date_to_string }}</a> {% if post.author %} ({{post.author}}) {% endif %}
      {{ post.excerpt }}
      <a href="{{ post.url }}">More about {{ post.title }}</a>
    </li>
  {% endfor %}
</ul>


You can subscribe to a [feed of the latest posts here](/feed.xml). 
