---
layout: page
title: systems
---
here are my daily wins lol.

<ul>
  {% assign all_systems = site.systems | sort: "date" | reverse %}
  {% for system in all_systems %}
    <li><a href="{{ system.url }}">{{ system.title }}</a></li>
  {% endfor %}
</ul>

## See also:
<a href="/systems/templates/">Templates for various stuff</a>