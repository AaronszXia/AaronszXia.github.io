---
layout: default
published: true
---

# Hi there, I'm Aaronsz Xia!

Welcome to my personal website! This site is a customization of Bootstrap 4.1.3, powered by Jekyll, hosted on GitHub.

You can find its source code [here](https://github.com/AaronszXia/jekyll-bootstrap) if you are interested in it.

Feel free to copy and re-use any and all of the code contained here without contacting me.

本网站涉及到的技术主要有

网站托管：[GitHub Pages](https://pages.github.com/)

网站生成：[Jekyll](https://jekyllrb.com)、[Liquid](https://shopify.github.io/liquid/ "An open-source template language")

网页样式：[Bootstrap](https://getbootstrap.com)、[Jekyll Bootstrap](http://jekyllbootstrap.com "The Definitive Jekyll Blogging Framework")

评论服务：[gitalk](https://gitalk.github.io/)

网页统计服务：[百度统计](https://tongji.baidu.com)

其他：[rss](https://zh.wikipedia.org/wiki/RSS "简易信息聚合")

## Here's the posts list:

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>
