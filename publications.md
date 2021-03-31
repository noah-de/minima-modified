---
title: Publications
layout: default
permalink: /publications/
---
<h1>Publications</h1>
{% for pub in site.publications %}
  <p><strong> <a href="{{ pub.url }}" >{{ pub.title }} </a></strong></p>
  <!-- {{ pub.content | markdownify }} -->
{% endfor %}

[back](./)
