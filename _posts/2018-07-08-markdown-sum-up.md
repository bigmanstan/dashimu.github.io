---
layout: post
categories: markdown
title: markdown 总结及最佳实践
date: 2018-07-08 23:14:31 +0800
description: markdown 总结及最佳实践，及插件，软件推荐
keywords: markdown
catalog: true
multilingual: false
tags: markdown
---

> 程序员写文章免不了用Markdown，自己参照文档，重新再写一遍，熟悉下规则。

### 自己喜欢的编辑器-VS Code

之前试下过其他的编辑器，都未能坚持。这一次我一定要成功的把Vs code用熟。

VS code 已经是众人推荐的编辑器了。 有非常丰富的扩展插件，比如说，markdown 的扩展插件 `Markdown All in One` , 把需要的功能集中一起，就能变成一个 markdown 编辑器。


> 详细说说 markdown 的语法规则

### 注释 - 跟HTML 一样

` <!-- 这里是注释 --> ` 

用快捷键是 `command + /`

### 标题

用  `#` :

```
# This is an <h1>
## This is an <h2>
### This is an <h3>
#### This is an <h4>
##### This is an <h5>
###### This is an <h6>
```

### 文字编辑

跟我们平常编辑文字一样。

文字变粗:  `**This text is in bold.**` , 快捷键为 `command + b`

文字斜体:  `*This text is in italics.*`, 快捷键为 `command + i`

引用语 :    `> This is a block quote.`


### 列表

**用了插件，按enter健自动列表**

无序列表 ： 

```
* Item
* Item
* Another item
```


有序列表：

```
1. Item one
2. Item two
3. Item three
```

### 代码高亮

单行代码 用两个 ``

多行代码 用两个 ```



### 水平线

``` --- ```


### 超链接

`[Click me!](http://test.com/) `

### 图片

` ![This is the alt-attribute for my image](http://imgur.com/myimage.jpg "An optional title")`

这里配合用七牛的上传图片软件 **cuimage**，效率提高更多.

### 表格
```
 | Col1         | Col2     | Col3          |
 | ----------- | ------ | ------------ |
 | Left-aligned | Centered | Right-aligned |
 | blah         | blah     | blah          |
 
 ```

 ### To - do 列表

格式为：` - [ ] `

完成与否，用插件的快捷键 ` option + c`

```
- [ ] Not finish
- [x] Finished
```


> 未完待续