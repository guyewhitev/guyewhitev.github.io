---
layout: page
title: Home
permalink: /
---

{% include background.html %}

<style>
  header#main { display: none; }
  main, .page-content, .post-content, article {
    padding-top: 0 !important;
    margin-top: 0 !important;
  }
</style>

<div class="image-overlay-wrapper">
  <img src="{{ '/assets/home.jpg' | relative_url }}" alt="Lit Candle in hands">
  <div class="image-overlay-text">
    MAKING <br>
    A CHANGE <br>
    STARTS WITH YOU
  </div>
</div>

The aim of this website is to promote knowledge and awareness of current global problems, along with solutions that can be used in an attempt to make the world a better place. Though I feel that we already have many problems to deal with in our everyday lives without needing more, so that is why I decided to create this website, to show that anyone, whoever they are, can make an impact and difference in the world we live in. Every month I will continue to write about a new world problem and how you can make a difference.

{% assign latest = site.posts.first %}
<div class="issue-card">
  <p class="issue-date">This month's issue</p>
  <h3><a href="{{ latest.url | relative_url }}">{{ latest.title }}</a></h3>
  <p>{{ latest.content | strip_html | truncatewords: 30 }}</p>
  <p><a href="{{ '/subscribe/' | relative_url }}">Subscribe</a> to get next month's issue by email.</p>
</div>
