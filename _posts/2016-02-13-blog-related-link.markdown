---
layout: post
title:  "Github Pages + Jekyll 建博客站（小白教程）"
subtitle: "How to build a blog via Github Pages and Jekyll"
date:   2016-02-13 17:32:00
author: "Linkai"
header-img: "img/post-2016-02-13-april.jpg"
tags:
   - tech
   - 中文
   - blog
---

# 前言
----------------------------------
动力来自某日逛知乎的一个帖子，[准备自己建一个个人博客，有什么好的框架推荐？](https://www.zhihu.com/question/24179143/answer/26928915)
幸幸苦苦架个blog（都是抄的），不写个流水账怎么行！

# 正文
-------------------------------------

## 用哪个？github page和wordpress

我之前的blog是搭载在wordpress上面的，wordpress作为一个广为所知的强大个人信息发布工具，自然有它的优势：

* 现成的后台系统，强大的**动态**网站
* 成熟的模版插件机制
* 基本不用碰代码

当然了，麻烦也是有的：

* 你得专门买个空间给个人域名（什么？你有免费的。。）
* 你得维护这个空间（什么？有人免费带你维护？。。）
* 部署起来相对麻烦一些些（你是老手了？那当我没说。。）

github pages是则是完全不一样的：

* 它是**静态**网站，网页内容完全是本地生成的静态页面
* 你的数据都在github上托管，不用服务器买空间啦
* 轻量快速易部署

不过麻烦也不少

* 至少要懂一点git，懂一点前端知识（你是程序员？好那当我没说）
* 配置各类插件还是要求你得懂代码（你是程序员？好那我没说）

说了这么多，我这次为什么要迁移我的blog呢？很简单

> 人就是爱折腾！

要有所进步，就要不安现状，keep moving!

## github page部署入门链接导读
有三篇文章说的相当相当的清楚：

1. [搭建一个免费的，无限流量的Blog----github Pages和Jekyll入门](http://www.ruanyifeng.com/blog/2012/08/blogging_with_jekyll.html)
2. [打造你的 GitHub Pages 专属博客（小白教程）](http://azeril.me/blog/Build-Your-First-GitHub-Pages-Blog.html)
3. [使用Github Pages建独立博客](http://beiyuu.com/github-pages/)

对于这三篇文章，我的建议是

* 先全部泛读一遍
 - 第一篇文章其实完全没怎么说jekyll，dns和CNAME配置也讲的不大好
 - 第二篇文章很赞，也有jekyll多种模版可用，就是起点有点高
 - 第三篇文章说的比较泛啦，适合新人读一读
* 用第三篇文章前半部分配置你的github相关信息（如果你没有的话）
* 用第一片文章的简易例子先做一个简易的网站
* 决定自己做的时候，去godaddy买一个自己喜欢域名，
* 按照第二篇文章的内容，找一个合适的模版，fork／clone下来，开始建一个稍微好看点的网站
* 别忘记去DNSpod配置你的域名相关信息！尤其是最后www那一条，我配置的时候忘记了，导致我的[3w域名](www.xilinkai.com)还是连接到原来的服务器bluehost上面。。

## 部署
终于到我自己的总结步骤了！

* 你要有git. 我不大喜欢git在mac上面的客户端，terminal用的蛮好。**git like a geek!**
* 在自己的github上面建一个repository，或者去你心仪的模版repository fork一个过来
* 你要有jekyll. 没有的话gem install jekyll
* 完成相应_config.xml里面的内容配置
* 删掉模版或者他人博客里_posts和_imgs下面的私有内容
* 添加CNAME里面你的个人域名
* 去DNSpod添加A纪录和CNAME的纪录，仿照上面第二篇文章
* jekyll serve 这样你就能本地在localhost:4000看到你的网站原型了
* git add commit push! *我比较喜欢gh-pages这个brunch啦！这样你的io那个唯一主页还可以留作他用，或者以后用主页host，然后通过连接blog到你的gh-pages这边来*
* 去你自己域名看博客咯！好好写文章吧！

## 模版和CSS前端
模版的话，我喜欢这篇[Jekyll 博客主题精选](http://azeril.me/blog/Selected-Collection-of-Jekyll-Themes.html)
当然你也可以去[jekyllthemes](http://jekyllthemes.org/)找,只是我觉得良莠不齐，大海捞针。。
对了，可以观摩一下[羡辙杂俎](http://zhangwenli.com/blog/)，实在是太棒太棒了，每看必跪。。
最后最后，感谢[黄玄](huangxuan.me)大大的[模版](https://github.com/Huxpro/huxpro.github.io)提供，我的站点基本用了他提供的模版。。

## 关于博客写作格式markdown
我用的是[macdown](http://macdown.uranusjr.com/)客户端，目前感觉良好。
在简书上看到一个有意思的八卦，[Mac 下两款 Markdown 编辑器 Mou/MacDown 大 PK](http://www.jianshu.com/p/6c157af09e84)

## 其他
动态评论功能可以用disqus或者多说完成。

我打算继续完善这个博客，添加更多新功能。

也打算在github建一个自己的模版。


# 博客相关链接
------------------------------------

先开个日志记录这个建站过程中有用的链接，重要性依次递减

1. http://huangxuan.me/ 这个个人博客真是inspire me a lot！
2. http://zhangwenli.com/blog/
3. http://www.ruanyifeng.com/blog/2012/08/blogging_with_jekyll.html
4. http://azeril.me/blog/Build-Your-First-GitHub-Pages-Blog.html
5. http://azeril.me/blog/Selected-Collection-of-Jekyll-Themes.html
6. http://azeril.me/blog/Markdown-Syntax.html
7. http://cnfeat.com/blog/2014/05/10/how-to-build-a-blog/







## 常用参考

1. http://jekyllrb.com/docs/home/
