---
layout: page
title: milestones
permalink: /{{ site.baseurl }}/milestones/
---
here are my milestones lol.

<ul>
  {% assign all_miles = site.milestones | sort: "date" | reverse %}
  {% for mile in all_miles %}
      <li><a href="{{ mile.url }}">{{ mile.title }}</a> - {{ mile.date | date: "%b %-d, %Y" }}</li>
  {% endfor %}
</ul>