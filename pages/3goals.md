---
layout: page
title: goals
permalink: /goals/
---
here are all my goals lol

{% assign all_goals = site.goals | sort: "date" | reverse %}
{% for goal in all_goals limit:1 %}
  {{ goal.content }}
{% endfor %}

## All Goals:
<ul>
  {% assign all_goals = site.goals | sort: "date" | reverse %}
  {% for goal in all_goals %}
    <li><a href="{{ goal.url | relative_url }}">{{ goal.title }}</a></li>
  {% endfor %}
</ul>