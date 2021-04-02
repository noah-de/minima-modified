---
title: Publications
layout: default
permalink: /publications/
---
{% for pub in site.publications %}
  <p><strong> <a href="{{ pub.url }}" >{{ pub.title }} </a></strong></p>
  <!-- {{ pub.content | markdownify }} -->
{% endfor %}

[back](./)
