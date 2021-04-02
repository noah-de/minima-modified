---
title: Notes
layout: default
permalink: /notes/
---
{% for note in site.notes %}
  <p><a href="{{ note.url }}" >{{ note.title }} </a></p>
{% endfor %}
