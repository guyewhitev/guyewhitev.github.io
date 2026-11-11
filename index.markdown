---
layout: page
title: Home
permalink: /
---

{% include background.html %}

<style>
  header#main { display: none; }
</style>

# Promoting Global Awareness Around the World
        
![Candle in hands](assets/home.jpg)

*Photo by [Myriam-Fotos](https://pixabay.com/users/myriams-fotos-1627417/) on [Pixabay](https://pixabay.com)*
{: .photo-credit}

The aim of this website is to promote knowledge and awareness of current global problems, along with solutions that can be used in an attempt to make the world a better place. Though I feel that we already have many problems to deal with in our everyday lives without needing more, so that is why I decided to create this website, to show that anyone, whoever they are, can make an impact and difference in the world we live in. Every month I will continue to write about a new world problem and how you can make a difference.

{% assign latest = site.posts.first %}
<div class="issue-card">
  <p class="issue-date">This month's issue</p>
  <h3><a href="{{ latest.url | relative_url }}">{{ latest.title }}</a></h3>
  <p>{{ latest.content | strip_html | truncatewords: 30 }}</p>
  <p><a href="/subscribe/">Subscribe</a> to get next month's issue by email.</p>
</div>

### Making a change starts with you

In order to change the world, look at yourself and ask: "What can I do?" The answer is that even the smallest action can cause the biggest changes. 

### About the creator

I am currently a teenager, living in Oregon, and I am still trying to understand the world we live in. 
I remember feel in the past that I felt unqualified or too young to make any change, so I didn't. Now, I realize that anyone can make some kind of change, even if it is small.
