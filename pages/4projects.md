---
layout: page
title: projects
permalink: /projects/
---
here are my projects lol.

{% assign all_projects = site.projects | sort: "date" | reverse %}
{% for project in all_projects %}
  
<h2> <a href="{{ project.url | relative_url }}">{{ project.title }}</a></h2>
<ul>
<li>Started: {{ project.date | date: "%b %-d, %Y" }} </li>
<li>Status: {{ project.status }}</li>
<li>Tags: {{ project.tags }}</li>
</ul>

{% endfor %}
