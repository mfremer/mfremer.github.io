---
layout: page
title: Publications
permalink: /publications/
lang: en
---

{% for publication in site.publications reversed %}
  <h3>{{ publication.title }}</h3>
  <p>{{ publication.author }}</p>
  <p>{{ publication.conference }}</p>
  <img src="{{ publication.teaser }}">
  
  Go to the <a href="{{ publication.url }}">project page</a>.
{% endfor %}