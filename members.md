---
title: Members
layout: default
permalink: /members/

member_categories:
    - Faculty
    - PhD Students
    - Master Students
    - Undergrad Students
    - Post-doctoral Researchers
    - Software Engineer
---
{% for category in page.member_categories %}
  <h2>{{ category }}</h2>
  {% for person in site.members %}
   {% if person.portfolio-item-tag contains "current member" %}
  {% if person.portfolio-item-tag contains category %}
   <div> <img src="{{ person.avatar | absolute_url }}" class="blackandwhite"/>{{ person.title }}</div>
   {% endif %}
  {% endif %}
  {% endfor %}
{% endfor %}
<h2>Past members</h2>
{% for person in site.members %}
    {% unless person.portfolio-item-tag contains "current member" %}
<div>{{ person.title }}</div>
    {% endunless %}
{% endfor %}
