---
layout: page
title: wins
permalink: /wins/
---
here are my daily wins lol.

<ul>
  {% assign all_wins = site.wins | sort: "date" | reverse %}
  {% for win in all_wins %}
    <li><a href="{{ win.url }}">{{ win.title }}</a> - {{ win.date | date: "%b %-d, %Y" }}</li>
  {% endfor %}
</ul>