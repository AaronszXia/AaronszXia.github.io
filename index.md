---
layout: default
title: Aaronsz's Blog
description: 'A blog powered by Jekyll, hosted on GitHub.'
published: true
---

# Hi there, I'm Aaronsz Xia!

Welcome to my personal website! This site is a customization of Bootstrap 4.1.3, powered by Jekyll, hosted on GitHub.

You can find its source code [here](https://github.com/AaronszXia/jekyll-bootstrap) if you are interested in it.

Feel free to copy and re-use any and all of the code contained here without contacting me.

<!-- I am a student of <abbr title="Nanjing University of Posts and Telecommunications">NJUPT</abbr> by day, and a programmer by night. -->

<!-- It is my personal website and currently being updated not so actively, cause I am preparing for the postgraduate entrance examination. -->

## Here's the posts list:

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>
