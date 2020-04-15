# 关于这个项目的说明

[![GitHub stars](https://img.shields.io/github/stars/xionHung/xionhung.github.io.svg)](https://github.com/xionHung/xionhung.github.io/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/xionHung/xionhung.github.io.svg)](https://github.com/xionHung/xionhung.github.io/network)
[![GitHub issues](https://img.shields.io/github/issues/xionHung/xionhung.github.io.svg)](https://github.com/xionHung/xionhung.github.io/issues)
[![GitHub release](https://img.shields.io/github/release/xionHung/xionhung.github.io.svg)](https://github.com/xionHung/xionhung.github.io/releases)
[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/xionHung/xionhung.github.io/master/LICENSE)


**博客访问地址：[http://xionhung.github.io/](http://xionhung.github.io/)**。

## 目录

- [预览图](#预览图)
- [各部分详情](#各部分详情)
  - [主页 Home](#主页-home)
  - [归档页 Archives](#归档页-archives)
  - [分类页 Categories](#分类页-categories)
  - [标签页 Tags](#标签页-tags)
  - [收藏页 Collections](#收藏页-collections)
  - [展示页 Demo](#展示页-demo)
  - [关于页 About](#关于页-about)
  - [评论](#评论)
  - [目录 Contents](#目录-contents)
  - [代码高亮](#代码高亮)
  - [灯泡效果](#灯泡效果)
  - [移动端适配](#移动端适配)
  - [Footer](#footer)
  - [统计](#统计)
- [博客主题使用方法](#博客主题使用方法)
  - [1. 安装 ruby 和 jekyll 环境](#1-安装-ruby-和-jekyll-环境)
  - [2. 复制博客主题代码](#2-复制博客主题代码)
  - [3. 修改参数](#3-修改参数)
    - [基本信息](#基本信息)
    - [链接信息](#链接信息)
    - [评论信息](#评论信息)
    - [统计信息](#统计信息)
  - [4. 写文章](#4-写文章)
  - [5. 本地运行](#5-本地运行)
  - [6. 发布到 GitHub](#6-发布到-github)

## 预览图

先上预览图：

主页
![index](http://ww3.sinaimg.cn/large/7011d6cfjw1f3bdli86awj211k0oyqen.jpg)

文章页
![post](http://ww4.sinaimg.cn/large/7011d6cfjw1f3bdmzb9v6j210p0j7gwn.jpg)

## 各部分详情

### 主页 Home

主页默认展示 5 篇文章的摘要部分，用户点击标题或阅读全文后进入文章页。右侧为近期文章、分类和标签 3 块区域，用户可以继续在这部分添加区域，只需修改`index.html`即可。

### 归档页 Archives

按照年份归档文章。

### 分类页 Categories

按照文章的分类，显示文章。

### 标签页 Tags

按照文章的标签显示文章。

### 收藏页 Collections

本页是用`markdown`写的，用户可以收藏自己喜欢的文章链接。

### 展示页 Demo

使用 [Masonry](http://masonry.desandro.com/) 重写了瀑布流布局，响应式布局，更好的交互体验。

### 关于页 About

对个人和对本站的介绍，使用`markdown`写的。

### 评论

支持 [多说评论](http://duoshuo.com/) 和 [disqus](https://disqus.com/) 评论。

只需要在 `_config.yml` 修改相应的配置`short_name`即可，如下：

```yml
# comments
# two ways to comment, only choose one, and use your own short name
# 两种评论插件，选一个就好了，使用自己的 short_name
duoshuo_shortname: #xxx
disqus_shortname: xxx
```

### 目录 Contents

页面滚动时目录固定在屏幕右侧，若目录高度超出屏幕高度，目录产生滚动条。

### 代码高亮

随着 jekyll 的升级，目前代码高亮使用风格与 github 上的 markdown 写法一致。

### 灯泡效果

![light](http://ww3.sinaimg.cn/large/7011d6cfjw1f3be6y4vp3j209i02rweg.jpg)

可以看到导航按钮高亮时，下面的阴影效果，我把这个称为灯泡效果。

### 移动端适配

完美适配移动端。

![mobile](http://ww4.sinaimg.cn/large/7011d6cfjw1f3bebnzxkpj20ah0fzgp4.jpg)

### 统计

博客支持百度统计和 Google Analytics，只需在`_config.yml`中配置响应的 id 即可，代码如下。

```yml
# statistic analysis 统计代码
# 百度统计 id，将统计代码替换为自己的百度统计id，即
# hm.src = "//hm.baidu.com/hm.js?xxxxxxxxxxxx";
# xxxxx字符串
baidu_tongji_id: xxxxxxxxxxxx
google_analytics_id: UA-xxxxxxxx # google 分析追踪id
```

## 博客主题使用方法

欢迎使用这个主题，以下简单说一下使用方法。

### 1. 安装 ruby 和 jekyll 环境

这一步和第 5 步主要是为了让博客系统在本地跑起来，如果不想在本地运行，可以无视这两步，但我还是强烈建议试着先在本地跑起来，没有什么问题后再推送的 GitHub 上。

Windows 用户可以直接使用 [RubyInstaller](http://rubyinstaller.org/) 安装 ruby 环境。后续的操作中可能还会提示安装 DevKit，根据提示操作即可。

建议使用 [RubyGems 镜像- Ruby China](https://gems.ruby-china.org/) 安装 jekyll。

安装 jekyll 命令如下

```
gem install jekyll
```

详情可以查看 jekyll 官网。[https://jekyllrb.com/](https://jekyllrb.com/) 或 中文翻译版 jekyll 官网[http://jekyllcn.com/](http://jekyllcn.com/) （中文文档翻译落后于英文官网，有兴趣有时间的小伙伴可以参与翻译，为开源世界贡献一份力哦~）

在 mac OS X El Capitan 系统下安装可能会出现问题，解决方案详情见 jekyll 官网: [ https://jekyllrb.com/docs/troubleshooting/#jekyll-amp-mac-os-x-1011](https://jekyllrb.com/docs/troubleshooting/#jekyll-amp-mac-os-x-1011)

对 jekyll 本身感兴趣的同学可以看看 jekyll 源码: [https://github.com/jekyll/jekyll](https://github.com/jekyll/jekyll)

![jekyll logo](http://jekyllcn.com/img/logo-2x.png)

### 2. 复制博客主题代码

可以直接 clone 、下载 或 fork 这个仓库的代码即可

### 3. 修改参数

主要修改 `_config.yml` 中的参数和自己的网站小图`favicon.ico`

`_config.yml`文件中

#### 基本信息

主要用于网站头部 header。

```yml
# Site settings
title: xionHong技术专栏
brief-intro: Front-end Dev Engineer
baseurl: "" # the subpath of your site, e.g. /blog
url: "http://xionhung.github.io" # the base hostname & protocol for your site
```

#### 链接信息

主要用于网站底部 footer。

```yml
# other links
github_username: xionHung
email: xionhong@foxmail.com
weibo_username: 3178561351 #Hong熊

description_footer: 会敲点代码的熊!
```

#### 评论信息

获取`short_name`的方法：

访问 https://intensedebate.com

```yml
# comments
# intensedebate 为英文版本，毕竟是国外的东西，应该也有中文插件，上网自行搜索
intensedebate_comments: #控制是否要显示评论工具
intensedebate: # idcomments_acct
```

运行成功后，可以在 intensedebate 的后台管理页看到相关信息。

#### 统计信息

获取 百度统计 id 或 Google Analytics id 的方法：

访问 http://tongji.baidu.com/ 或 https://www.google.com/analytics/ 根据提示操作即可。当然，如果不想添加统计信息，这两个参数可以不填。

```yml
# statistic analysis 统计代码
# 百度统计 id，将统计代码替换为自己的百度统计id，即
# hm.src = "//hm.baidu.com/hm.js?xxxxxxxxxxxx";
# xxxxx字符串
baidu_tongji_id: cf8506e0ef223e57ff6239944e5d46a4
google_analytics_id: UA-72449510-4 # google 分析追踪id
```

成功后，进入自己的百度统计或 Google Analytics 后台管理，即可看到网站的访问量、访客等相关信息。

### 4. 写文章

`_posts`目录下存放文章信息，文章头部注明 layout(布局)、title、date、categories、tags、author(可选)、mathjax(可选，点击[这里](https://www.mathjax.org/)查看更多关于`Mathjax`)，如下：

```
---
layout: post
title:  "对这个 jekyll 博客主题的改版和重构"
date:   2016-03-12 11:40:18 +0800
categories: jekyll
tags: jekyll 端口 markdown Foxit RubyGems HTML CSS
author: Haoyang Gao
mathjax: true
---
```

下面这两行代码为产生目录时使用

```
* content
{:toc}
```

文章中存在的 4 次换行为摘要分割符，换行前的内容会以摘要的形式显示在主页 Home 上，进入文章页不影响。

换行符的设置见配置文件`_config.yml`的 excerpt，如下：

```yml
# excerpt
excerpt_separator: "\n\n\n\n"
```

使用 markdown 语法写文章。

代码风格与 GitHub 上 README 或 issue 中的一致。使用 3 个\`\`\`的方式。

### 5. 本地运行

本地执行

```
jekyll s
```

显示

```
Configuration file: E:/GitWorkSpace/blog/_config.yml
            Source: E:/GitWorkSpace/blog
       Destination: E:/GitWorkSpace/blog/_site
 Incremental build: disabled. Enable with --incremental
      Generating...
                    done in 6.33 seconds.
  Please add the following to your Gemfile to avoid polling for changes:
    gem 'wdm', '>= 0.1.0' if Gem.win_platform?
 Auto-regeneration: enabled for 'E:/GitWorkSpace/blog'
Configuration file: E:/GitWorkSpace/blog/_config.yml
    Server address: http://127.0.0.1:4000/
  Server running... press ctrl-c to stop.
```

在本地访问 localhost:4000 即可看到博客主页。

若安装了 Foxit 福昕 pdf 阅读器可能会占用 4000 端口，关闭 Foxit 服务 或切换 jekyll 端口即可解决。详情见文章：[对这个 jekyll 博客主题的改版和重构](http://xionhung.github.io/2016/03/12/jekyll-theme-version-2.0/)

若正在使用全局代理，可能会报错 502，关闭全局代理即可。

### 6. 发布到 GitHub

没什么问题，推送到自己的博客仓库即可。
