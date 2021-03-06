# 关于这个Jekyll模板主题
---
## 标签

+ 首页: 博客首页
+ 博文分类: 按照categories对文章进行分类
+ 标签分类: 按照tags对文章进行分类



---

## 功能简介

### 提供全文搜索

博客使用[`Simple-Jekyll-Search`](https://github.com/christian-fei/Simple-Jekyll-Search)提供全文搜索功能。

### 提供百度统计功能

博客使用[百度统计](https://tongji.baidu.com/web/welcome/login)提供统计功能。具体操作方法在官网有详细介绍。

### 提供不蒜子pv/uv计数器

[不蒜子](http://busuanzi.ibruce.info/)可以提供pv/uv的计数。好处在于可以在界面上显示访问量。


### 添加社会化评论功能
博客采用第三方评论平台[Gitment](https://github.com/imsun/gitment)


### 使用canvas实现首页动态效果

### 使用日历控件显示当前日期


---

## 博客使用方法

初识Jekyll博客，有必要了解[Jekyll](https://jekyllrb.com/)有关知识。

### 下载本博客源码

欢迎fork, clone and star。

### 修改_config.yml文件

包括相关的一些设置参数，包括banner/motto/description等。

> 直接修改便会生效。

### 写文章

文章放在`_post`文件夹下，可创建自命名文件夹。支持markdown编写，提供`post`(知识共享署名-非商业性使用-禁止演绎 4.0 国际许可协议)/`original`(原创文章)两种方式。

文件命名示例如下:

```
2017-03-23-More-of-prototype.md
```

文章首部字段为:

```markdown
---
layout: post
title: "再谈原型和继承"
date: 2017-03-23 09:00:00 +0800
categories: 研究生涯
tag: JavaScript
---
* content
{:toc}
```

> 备注一: Jekyll使用时间对文章进行排序，所以无论如何建立文件夹和文件夹命名都行，你开心就好

> 备注二: 未完成的草稿文章可以放在`_draft`文件夹中

### 运行

使用下面命令可直接运行:

```bash
$ jekyll s
```

会开启jekyll服务器，监听在`http://127.0.0.1:4000/`，使用浏览器访问呢。

不想查看效果，可直接bulid。

```bash
$ jekyll build
```


---

## License

[CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/)