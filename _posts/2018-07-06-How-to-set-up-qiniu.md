---
layout: post
categories: 域名
title: 七牛的Https二级域名如何设置
date: 2018-07-06 17:14:31 +0800
description: 七牛的Https域名如何设置
keywords: 域名 七牛
catalog: true
multilingual: false
tags: 域名
---

> 因为要镜像有https图片，对七牛的域名绑定不熟悉，花费一些时间，知道了他们的规则后，很快就搞定。



### 确定域名是ssl

本来我的域名是ssl，刚开始直接用主域名作为回源域名，我设置不当，导致网站404. 
所以， **对七牛存储空间的自定义域名（自定义域名建议使用二级域名）进行 CNAME 配置**

比如我要这样的二级: **image.myname.com**

二级域名也要SSL，还好七牛有免费的ssl申请，按照提示，也是很快生成，设置好了。

### 七牛域名管理

 - 选择 **普通域名**  
 - 域名为刚刚设置的二级域名
 - HTTPS 选择设置的二级域名

![](https://image.hanguotudi.com/20180706183156_QuqW2Y_Screenshot 2018-07-06 18.30.51.jpeg)

### 域名的CNAME解析

以前的DNSPod ,现在被腾讯云合并，我是这样做域名的CNAME解析的：


- 主机记录：填写 **image**
- 记录类型：**CNAME**
- 线路类型： 默认即可
- 记录值：填写七牛提供的 CNAME 值

![](https://image.hanguotudi.com/20180706183748_CyOK91_Screenshot 2018-07-06 18.37.33.jpeg)

### 回源配置

填写二级域名 **image.myname.com**

另外，在镜像存储设置中，这里不需要填写 **镜像源**

### 推荐一个Mac客户端的七牛上传工具：Cuimage

对于用 Markdown 写作的人，图片是一个麻烦的操作，此工具解决了这个问题.
简单的设置，上传图片后，自动生成 Markdown 格式。非常方便。

![](https://image.hanguotudi.com/20180706185710_3I1KX6_687474703a2f2f6f68636f71626638652e626b742e636c6f7564646e2e636f6d2f32303137303231303136303432325f30724f3472385f6375496d61676544656d6f2e676966.gif)


> 完