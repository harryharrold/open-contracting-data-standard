---
layout: blog
title: The Data Standard Blog
---

<ul>
  {% for post in site.posts %}
  <li>
    <h2><a href="{{site.baseurl}}{{ post.url }}">{{ post.title }}</a></h2>
    <p><time datetime="{{post.date}}">{{ post.date  | date_to_string }}</time>{% if post.author %} <span aria-hidden="true">&middot;&middot;&middot;</span> <span class="author">{{post.author}}</span>{% endif %}</p>
    {{ post.excerpt }}
    <p><a href="{{site.baseurl}}{{ post.url }}}">More about {{post.title}} &hellip;</a></p>
  </li>
  {% endfor %}
</ul>
