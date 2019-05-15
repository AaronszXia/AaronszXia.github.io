---
layout: default
published: true
---
{% include JB/is_production %}
    
{% if is_production != true %}
  <h3>This is Private</h3>
  <p>I love to watch television in my undies. Don't tell anyone!</p>
{% endif %}

# 你好，我叫**夏龙飞**!

目前是[皇家邮电大学](http://www.njupt.edu.cn "南京邮电大学")软件工程专业大三学生，现任**管理学院科学与技术协会科研中心主任**。

欢迎访问我的个人网站！这个网站采用 Jekyll 技术生成静态网页文件，托管于 GitHub Pages 上，由 Bootstrap 提供网页响应式布局。网站所使用的图标来源于[Font Awesome](https://fontawesome.com)在线图标库（由于服务器位于国外，初次打开本网站加载图标的时间可能会画一点时间）。

作为一个理工男，我并不认为我的审美足够地好。因此，在保证此网站的所有页面能够正常、恰当地工作的前提下，我极少使用自定义样式，其余全采用 Bootstrap 和 Jekyll 的默认样式。

希望你喜欢它的页面布局。

这个网站的文章页面底部有基于 gitalk 项目的评论板块，欢迎在这儿评论我的文章。

它的源码已经在 GitHub 上开源，如果你感兴趣，可以在[这儿](https://github.com/aaronszxia/aaronszxia.github.io)找到它。

你可以自由地使用这个项目里的部分或者全部代码，没有任何版权限制。当然，如果你使用的时候能够署上我的名字和添加一个指向这个网站的超链接，我将会非常感谢。
{% if is_production != true %}
Welcome to my personal website! This site is a customization of Bootstrap 4.1.3, powered by Jekyll, hosted on GitHub.

You can find its source code [here](https://github.com/AaronszXia/jekyll-bootstrap) if you are interested in it.

Feel free to copy and re-use any and all of the code contained here without contacting me.
{% endif %}
这个网站使用到的服务和涉及到的技术主要有：
- 网站托管 > [GitHub Pages](https://pages.github.com/)
- 网站生成 > [Jekyll](https://jekyllrb.com)、[Liquid](https://shopify.github.io/liquid/ "An open-source template language")
- 网页样式 > [Bootstrap](https://getbootstrap.com)、[Jekyll Bootstrap](http://jekyllbootstrap.com "The Definitive Jekyll Blogging Framework")
- 评论服务 > [gitalk](https://gitalk.github.io/)
- 网页统计服务 > [百度统计](https://tongji.baidu.com)
- 图标 > [Font Awesome](https://fontawesome.com)
- 其他 > [rss](https://zh.wikipedia.org/wiki/RSS "简易信息聚合")

<!-- ## Here's the posts list: -->

## 这是我近期原创或转载的一些文章:

<ul>
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>
