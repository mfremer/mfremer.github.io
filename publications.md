---
layout: page
title: Publications
---

{% for publication in site.publications %}
  <h2>{{ publication.title }}</h2>
  <p>{{ publication.author }}</p>
  <img src="{{ publication.teaser }}" alt="PCBend teaser">
  <p>Go to the <a href="{{ publication.url }}">project page</a>.</p>
{% endfor %}
