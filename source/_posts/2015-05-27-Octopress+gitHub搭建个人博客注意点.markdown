---
layout: post
title: "Octopress+gitHub”
date: 2015-05-27 21:31:00 +0800
comments: true
categories: 
---
# Octopress+gitHub搭建个人博客注意点

# 推荐博客
网址：<http://segmentfault.com/a/1190000000364677>

# 更换ruby源
gem经常很慢，或者被墙，可以替换成taobao的源进行解决
$ gem sources --remove http://rubygems.org/  
$ gem sources -a http://ruby.taobao.org/  
$ gem sources -l  
 CURRENT SOURCES 
  http://ruby.taobao.org  
**请确保只有** ruby.taobao.org  
如此还不行，请在Octopress目录下找到gemfile（gem将要安装的一些程序）使用VI命令或者文本编辑器把http://rubygems.org/也替换成http://ruby.taobao.org/ 
# 删除Octopress源代码中被墙的网址使用
如facebook,如twitter，之类。这些会有可能会在我们访问自己博客的时候被访问从而影响我们博客的加载速度甚至导致部署后访问不了。罪魁祸首就是GFW.
位置在：config.yml; /source/_includes/custom/head.html;
如果你不小心文件删除head.html，而部署了.头文件已经加载到不同的方的head.html中了，需要全局查找使用过google api的head.html不逐一把他们删除
# 把自己的微博放入博客
需要设置自己的个性域名；在微博设置->账号设置里面就可以看到个性域名的设了。
# 评论插件Disqus的安装
填入注册disqus测后，也有类似微博个性域名的要设置，这个并不是你的登入账号，而是单独在disqus网站申请的！
