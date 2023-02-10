---
layout: archive
title: PhD Blog
permalink: /PhD%20Blog/
author_profile: true
---
## PhD Blog
Welcome to my blog! If you're thinking about applying for a PhD, then I hope that these posts will be useful to you!

{% include base_path %}
{% capture written_year %}'None'{% endcapture %}
{% for post in site.posts %}
  {% capture year %}{{ post.date | date: '%Y' }}{% endcapture %}
  {% if year != written_year %}
    <h2 id="{{ year | slugify }}" class="archive__subtitle">{{ year }}</h2>
    {% capture written_year %}{{ year }}{% endcapture %}
  {% endif %}
  {% include archive-single.html %}
{% endfor %}