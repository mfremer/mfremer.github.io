---
layout: page
title: Publications
---

{% for publication in site.publications %}
  <h3>[{{ publication.conference }}] {{ publication.title }} (<a href="{{ publication.url }}">Project page</a>)</h3>
  <p>{{ publication.author }}</p>
  <img src="{{ publication.teaser }}" alt="PCBend teaser">
{% endfor %}
