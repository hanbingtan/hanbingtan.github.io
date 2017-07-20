---
layout: post
title: "github pages+jekyll搭建个人博客(一)"
date: 2016-09-05 10:48:00 +0800 
categories: 博客搭建
tag: jekyll
---
* content
{:toc}

`github博客`搭建方案

<!-- more -->

最近初学github  pages搭建博客，看到了几类教程，分别是搭建Jekyll 博客和搭建hexo博客。现在在这里主要介绍一下在windows上如何搭建Jekyll 博客。

搭建过程参考了[《jekyll安装及写静态博客》](http://www.tuicool.com/articles/7Vz6BzJ)这篇文章，由于版本不同的原因，搭建不成功，但是还是十分感谢作者。在此重新梳理下搭建过程，方便大家少走一些弯路。
# 本地jekyll环境配置
1.下载并且安装 ruby 和 DEVELOPMENT KIT
官方下载地址 [http://rubyinstaller.org/downloads/](http://rubyinstaller.org/downloads/)

1.1下载并安装rubyinstaller-2.1.9-x64.exe到C:\Ruby目录
**notice**：安装的时候，记得勾选添加ruby到环境变量，如下图所示：
![graph]({{ '/pic/博客搭建/ruby-evn.png' | prepend: site.baseurl }})

1.2下载并解压对应的rubydevkit： DevKit-mingw64-64-4.7.2-20130224-1432-sfx .exe到C:\rubydevkit目录
解压了rubydevkit之后，进入该目录下通过初始化来创建 config.yml 文件
```
cd C:\rubydevkit
ruby dk.rb init
ruby dk.rb install
```
2.安装 Jekyll gem
```
gem install jekyll -v 2.1.0
```
3.安装rdiscount，这个是用来解析Markdown标记的解析包
```
gem install rdiscount
```
4.安装 Pygments
Jekyll 里默认的语法高亮插件是 [Pygments](http://pygments.org/)。 它需要安装 Python并在网站的配置文件_config.yml里将highlighter的值设置为pygments。
4.1下载并安装python环境
下载[python2.7](https://www.python.org/downloads/)，安装并且配置python的环境路径
4.2安装 Easy Install
打开链接[ez_setup](https://bootstrap.pypa.io/ez_setup.py)，并且右键另存为ez_setup.py，然后运行该文件。
4.3安装配置Pygments
进入C:\Python27\Scripts（python安装目录）执行easy_install Pygments。安装Pygments
```
easy_install Pygments
```
如果没报错的话，congratulations！你的jekyll环境就搭建好了。

# 启动 Jekyll
按照官方的 [Jekyll 快速开始手册](http://jekyllrb.com/docs/quickstart/) 的步骤， 一个新的 Jekyll 博客可以被建立并在[localhost:4000](http://localhost:4000/)浏览。
```
jekyll new blog
cd blog
jekyll serve
```

![graph]({{ '/pic/博客搭建/jekyll-success.png' | prepend: site.baseurl }})
