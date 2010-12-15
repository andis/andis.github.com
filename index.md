---
layout: basic
title: Home
---

Hello World
==========

As with every public git repository, history is being made.

Posts
==========

<div class="listofposts">
{% for post in site.posts %}
    <div class="post">
    <p class="date">{{ post.date | date: "%B %e, %Y" }}</p>
    <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
    <p>{{ post.excerpt }} <a href="{{ post.url }}" class="linktopost">more…</a></p>
    </div>
{% endfor %}
</div>
