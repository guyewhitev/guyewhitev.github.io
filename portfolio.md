---
layout: page
title: Monthly Issue
permalink: /monthly-issue/
---
{% include background.html %}

# This Month’s Issue

{% for post in site.posts %}
<div class="issue-card">
  <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
  <p class="issue-date">{{ post.date | date: "%B %Y" }}</p>
  <p>{{ post.content | strip_html | truncatewords: 30 }}</p>
</div>
{% endfor %}