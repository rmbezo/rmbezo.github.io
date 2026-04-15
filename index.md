---
layout: default
title: Posts
---

## Posts

<ul class="post-list">
  {% for post in site.posts %}
    <li class="post-item">
      <time class="post-date" datetime="{{ post.date | date_to_xmlschema }}">
        {{ post.date | date: "%b %d, %Y" }}
      </time>
      <a class="post-link" href="{{ post.url | relative_url }}">
        {{ post.title | escape }}
      </a>
    </li>
  {% endfor %}
</ul>

