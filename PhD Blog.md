---
title: PhD Blog
layout: home
nav_order: 3
---
## PhD Blog
Welcome to my blog! If you're thinking about applying for a PhD, then I hope that these posts will be useful to you!

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>