---
layout: page
title: reflections
permalink: /reflections/
---
here are my reflections lol.

<ul>
  {% assign all_reflections = site.reflections | sort: "date" | reverse %}
  {% for reflection in all_reflections %}
    <li><a href="{{ reflection.url }}">{{ reflection.title }}</a> - {{ reflection.date | date: "%b %-d, %Y" }}</li>
  {% endfor %}
</ul>