---
layout: page
title: systems
permalink: /{{ site.baseurl }}/systems/
---
here are my systems lol.

<ul>
  {% assign all_systems = site.systems | sort: "date" | reverse %}
  {% for system in all_systems %}
    <li><a href="{{ system.url }}">{{ system.title }}</a></li>
  {% endfor %}
</ul>

## See also:
<a href="/systems/templates/">Templates for various stuff</a>