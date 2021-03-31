---
title: Sponsors
layout: default
permalink: /sponsors/
---
<h1>Sponsors</h1>
{% for sponsor in site.data.sponsors %}
<div class="grid__item">
  <a href="{{ sponsor.url }}">
  <img width="200px"  src="/assets/images/logos/{{ sponsor.logo }}" alt="{{ sponsor.name }}"></a>
  </div>
{% endfor %}
