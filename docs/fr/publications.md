---
layout: page
title: Publications
permalink: /publications/
lang: fr
---

{% for publication in site.publications %}
  <h3>{{ publication.title }}</h3>
  <p>{{ publication.author }}</p>
  <p>{{ publication.conference }}</p>
  <img src="{{ publication.teaser }}">
  
  Aller à la <a href="{{ publication.url }}">page du projet</a>.
{% endfor %}