---
layout: page
title: Home
permalink: /
---

{% include background.html %}

<style>
  header#main, .title-padder { display: none !important; }
  .content, section, article, .post-content { padding-top: 0 !important; margin-top: 0 !important; }
  .image-overlay-wrapper {
    display: grid !important;
    grid-template-areas: "stack" !important;
    width: 100vw !important;
    height: 100vh !important;
    position: relative !important;
    left: 50% !important; right: 50% !important;
    margin-left: -50vw !important; margin-right: -50vw !important;
    margin-bottom: 40px !important;
  }
  .image-overlay-wrapper img {
    grid-area: stack !important; width: 100% !important; height: 100% !important;
    object-fit: cover !important; object-position: center !important;
    display: block !important; margin: 0 !important;
  }
  .image-overlay-text {
    grid-area: stack !important; align-self: start !important; justify-self: start !important;
    margin: 125px !important; max-width: calc(100% - 250px) !important;
    font-size: 5.25rem !important; font-weight: bold !important; line-height: 1.2 !important;
    text-align: left !important; color: rgba(127, 117, 117, 0.98) !important; z-index: 2 !important;
  }
  @media (max-width: 768px) {
    .image-overlay-text { font-size: 2.75rem !important; margin: 40px !important; max-width: calc(100% - 80px) !important; }
  }
</style>

<div class="image-overlay-wrapper">
  <img src="{{ '/assets/home.jpg' | relative_url }}" alt="Lit Candle in hands">
  <div class="image-overlay-text">MAKING <br> A CHANGE <br> STARTS WITH YOU</div>
</div>

The aim of this website is to promote knowledge and awareness of current global problems and solutions. Every month I will highlight a new issue and how you can make a difference.

{% assign latest = site.posts.first %}
<div class="issue-card">
  <p class="issue-date">This month's issue</p>
  <h3><a href="{{ latest.url | relative_url }}">{{ latest.title }}</a></h3>
  <p>{{ latest.content | strip_html | truncatewords: 30 }}</p>
  <p><a href="{{ '/subscribe/' | relative_url }}">Subscribe</a> to get next month's issue by email.</p>
</div>
