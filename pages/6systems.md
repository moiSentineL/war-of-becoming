---
layout: page
title: systems
permalink: /systems/
---
here are my systems lol.

<ul>
  {% assign all_systems = site.systems | sort: "date" | reverse %}
  {% for system in all_systems %}
    <li><a href="{{ system.url | relative_url }}">{{ system.title }}</a></li>
  {% endfor %}
</ul>
