---
layout: page
title: Monthly Issue
permalink: /monthly-issue/
---
{% include background.html %}

# This Month's Issue

<ul>
{% for post in site.posts %}
  <li><a href="{{ post.url | relative_url }}">{{ post.title }}</a> ({{ post.date | date: "%B %Y" }})</li>
{% endfor %}
</ul>

