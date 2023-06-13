---
title: practice_markdown
date: 2023-06-06 15:48:24
tags:
- markdown
categories: 
- tool
mathjax: true
---


<!-- @import "[TOC]" {cmd="toc" depthFrom=1 depthTo=6 orderedList=false} -->

<!-- code_chunk_output -->

- [编写markdown](#编写markdown)
  - [语法](#语法)
    - [标题(这就是)](#标题这就是)
    - [强调](#强调)
    - [列表](#列表)
    - [插入图片](#插入图片)
    - [链接](#链接)
    - [引用](#引用)
    - [分割线](#分割线)
    - [行内代码](#行内代码)
    - [代码块](#代码块)
    - [TOC](#toc)
      - [这个没有排除](#这个没有排除)
    - [任务列表](#任务列表)
  - [表格](#表格)
    - [Emoji](#emoji)
    - [标记](#标记)
      - [上标](#上标)
      - [下标](#下标)
      - [脚注](#脚注)
      - [缩略](#缩略)
      - [标记](#标记-1)
      - [Admonition 告诫](#admonition-告诫)
      - [数学](#数学)
  - [相关主题](#相关主题)

<!-- /code_chunk_output -->



# 编写markdown

由于本自建博客都是用markdown去写，所以想写篇教程使用 VS + Markdown Preview Enhanced 插件完成，这款插件旨在让你拥有飘逸的Markdown写作体验。

## 语法

### 标题(这就是)


### 强调

这是 *斜体字*
这是 **粗体** 
这是 __粗体__
这是 __*加粗斜体组合*__
这是 ~~删除~~

### 列表

- 编程语言
    - Java
        - 对象
            - Object
    - Python
        - 开发框架
            - flask
            - Django
        - 函数
            - print
    - Go

### 插入图片

![熊猫人表情](../imgs/1.jpg)

Ctrl+Shift+P 输入Image Helper， 可以选择Image Helper插入

![飞书20221202-172006](https://i.imgur.com/Zmzo7CY.jpg)

### 链接
[财富密码](https://prs1022.github.io/)

### 引用

> 人们真正注意到你的时候，不是第一眼看到你站在那里，而是发现过了这么久你居然还在那里。

### 分割线

---
我与上面切割了！ 


### 行内代码

用python打印一个helloworld怎么写？
是不是 `Print("hello world")` 才对。

### 代码块

``` java
System.out.println("hello world")
```

``` go
import {
    "fmt"
}
fmt.printf("hello world")
```

显示代码行数

``` javascript {.line-numbers}
function add(x,y){
    return x+y
}
```

高亮代码行

``` javascript {highlight=2}
var x=1,y=2
c = add(x,y)
console.log(c)
```

### TOC 
我喜欢这个功能，ctrl+shift+P打开命令面板 输入Create Toc，选择后就可以创建了。

并且它是可以根据你更改内容自动更新的。

#### 这个是被排除的标题 {ignore=true}
#### 这个没有排除

### 任务列表

- [x] 早饭吃了吗
- [x] 中饭吃了吗
- [ ] 学习了吗
- [x] 晚饭吃了吗


## 表格

First Header | Second Header 
------------ | -----------
Cell1 | Cell2
Cell3 | Cell4

合并单元格 (需要在插件设置中打开 __enableExtendedTableSyntax__ )
- 行合并 (> 或者 empty)
- 列合并 (^)

First Header | Second Header 
------------ | -----------
> | Cell2
> | Cell4

First Header | Second Header 
------------ | -----------
Cell1 | Cell2
^ | Cell4


### Emoji 
:smile:
:fa-car:
### 标记
#### 上标
30^o^

#### 下标
H~2~O

#### 脚注
Content [^1]

[^1]: Hi! This is a footnote

#### 缩略
*[HTML]: Hyper Text Markup Language
*[W3C]: World Wide Web Consortium
The HTML specification
is maintained by the W3C.

#### 标记
==我被标记了==

#### Admonition 告诫

!!! note this is the 告诫标题
    这是告诫主体

#### 数学
行内数学表达式 $ x^3 + y^3 = z^3 $

块表达式
$$
\sum_{n=1}^{100}n =?
$$

## 相关主题

在插件的设置中，我设置了预览的主题色和代码的背景色。整个设置内容非常多。详细的[参考](https://shd101wyy.github.io/markdown-preview-enhanced/#/zh-cn/markdown-basics)。

写完发现有些不能在github page上正确解析呀， 数学公式不能展示有点遗憾。

