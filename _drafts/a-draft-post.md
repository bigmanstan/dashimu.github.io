---
layout: post
categories: jekyll
title: Jekyll 搭建静态博客
date: 2018-07-05 23:14:31 +0800
description: 记录一下使用 jekyll 创建静态博客的过程
keywords: jekyll
catalog: true
multilingual: false
tags: Linux git 
---

> 花了一些时间，重新把编程技术的博客建设完成，我机器是用Macbook 笔记本的，记录一下过程：

### 一，准备工作

- 安装 homebrew 
- 安装 rbenv （Ruby管理工具，并可切换版本）
- 安装 ruby


### 二，搭建 jekyll

jekyll 搭建静态博客非常简单，只需要找一套可用的主题，然后安装好相关依赖即可，以下以 mritd.github.io 的主题为例

#### 2.1、clone 主题

``` sh
git clone git@github.com:mritd/mritd.github.io.git
```

#### 2.2、安装 jekyll

``` sh
# 进入主题目录
cd mritd.github.io
# 安装 jekyll 等
bundle install
```

#### 2.3、启动并修改

jekyll 等组件安装完成后便可直接启动预览博客

``` sh
# 启动 jekyll  
bundle exec jekyll serve
```

### 三、推送到 Github

**首先在 Github 上创建 `用户名.github.io` 项目，如 `dashimu.github.io`，然后删除刚刚下载主题目录下的 `.git` 目录，在执行 `git init` 初始化一下 git 仓库，最后将 master 地址指向新建的仓库地址推送即可；Github 本身也是使用 jekyll 进行生成，所以会自动识别并生成博客；最后访问 `http://用户名.github.io` 即可；**