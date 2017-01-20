layout: post
title: "Javascript History"
subtitle: "Javascript的诞生历史"
date: 2017-01-03 17:35:02
author: "mslinzz"
header-img: "bg-js.jpg"
tags:
    - javascript
---


> 前言

前端工程师, 很多时候都被问起, 你的js怎么样, 只能支支吾吾一下: 哎呦, 不错呦~ 其实总是没有一个总体的认知, 记忆很微浅, 所以就开始决定, 深入攻克一下 Javascript.

这个专栏, 会陆续记载我学习js的过程. 可以在我的 [Tags-Javascript学习记录](http://mslinzz.com/tags/#javascript) 中查看其他内容.

本篇主要记录:

- Javascript 的起源, 因何而生, 如何发展, 现状如何
- Javascript 与 ECMAScript 之间的关系
- DOM(Document Object Model, 文档对象模型), BOM(Broswer Object Model, 浏览器对象模型)
- ECMA(European Computer Manufacturer's Association, 欧洲计算机制造商协议) 与 W3C(World wide Web Consortium, 万维网联盟)制定的一些相关标准

> Javascript 历史回顾

Javascript 诞生于 1995年. 当时, 它的主要目的是处理以前由服务器端语言(如Perl)负责的一些输入验证操作. 在 Javascript 问世之前, 必须把表单数据发送道服务器端才能确定用户是有没有填写某个必填域, 是否输入了无效的值.

NetScape Navigator (网页浏览器) 希望通过 Javascript 解决这个问题. 自此, Javascript 逐渐成为市面上常见浏览器必备的一项特色功能. 今天的Javascript已经成为一门功能全面的编程语言, 能够处理复杂的计算机交互, 拥有了闭包, 匿名函数, 甚至元编程等特性. 作为Web的一个重要组成部分.

当时就职与NetScape(美国网景公司)的 Brendan Eich, 开始着手为计划于 1995年2月发布的 NetScape Navigator 2 开发一种名为 LiveScript 的脚本语言 -- 该语言将同时在浏览器何服务器中使用, 为了赶在发布日期前完成 LiveScript 的开发, NetScape 与 Sun 公司建议了一个开发联盟. 在 NetScape Navigator 2 正式发布前夕, NetScape 为了搭上媒体热炒 Java 的顺风车, 临时把 LiveScript 改名为 javaScript.

由于 Javascript 1.0 获得了巨大的成功, NetScape 随即在日后的 NetScape Navigator 3 中发布了 Javascript 1.1, 关注度屡创新高.

与此同时, 微软决定与 Navigator 竞争, 在 Internet Explorer 3 中加入了名为 JScript 的实现(为了避开授权问题).

这个时候, 就出现了 Javascript 和 JScript, 两个版本不同的局面暴露了诸多问题.

1997年, 以 Javascript 1.1 为蓝本的标准化建议提至 ECMA (欧洲计算机协会). 该协会指定39号技术委员会负责 '标准化一种通用, 跨平台, 供应中立的脚本语言的语法和语义'.
TC39由来自 Netscape, Sun, 微软, Borland及其他关注脚本语言发展公司的程序员组成. 他们经过数月的努力完成了 ECMA-262 (定义名为 ECMAScript) 的新脚本标准语言.

> Javascript 与 ECMAScript 之间的关系

由上小节得知, ECMAScript 是实现对 Javascript 标准化各个内容的语言的核心描述. 由 ECMA-262定义.

所以就有后来大家说的 ES5, ES6 等, 其实之前还有 1, 2, 3, 4

一个标准的 Javascript 有三个不同的组成部分:
- 核心 (ECMAScript)
- 文档对象模型 (DOM)
- 浏览器对象模型 (BOM)

> DOM(Document Object Model, 文档对象模型)
> BOM(Broswer Object Model, 浏览器对象模型)

DOM, 提供访问何操作网页内容的方法和接口. 是针对 XML 但经过扩展用于 HTML 的应用程序编程接口 (API, Application Programming Interface). DOM 把整个页面映射为一个多层节点结构. HTML 或 XML 页面中的每个组成部分都是某种类型的节点, 这些节点又包含不同类型的数据.
如下面, 大家所熟悉的:

```html
<html>
    <head>
        <title> Hello Html </title>
    </head>
    <body>
        <p> some message here... </p>
    </body>
</html>
```

通过 DOM 创建的这个标示文档的树形图, 开发人员获得了控制页面的内容和结构的主动权. 借助 DOM 提供的 API, 开发人员可以轻松自如的删除, 添加, 替换何修改任何节点.

BOM, 提供与浏览器交互的方法和接口. 是支持可访问和操作浏览器窗口的浏览器对象模型. 开发人员使用 BOM 可以控制浏览器显示的页面以外的页面.

- 弹出新浏览器窗口的功能;
- 移动, 缩放, 关闭浏览器的功能;
- 提供浏览器详细信息的 navigator 的功能;
- 提供浏览器所加载页面的详细信息的 location 对象;
- 提供用户显示器分辨率信息的 screen 对象;
- 对 cookies 的支持;
- 像 XMLHttpRequest 和 IE 的 ActiveXObject 这样的定义.

> 相关标准
> ECMA(European Computer Manufacturer's Association, 欧洲计算机制造商协议)
> W3C(World wide Web Consortium, 万维网联盟)

ECMA 为我们制定了 Javascript 的核心标准;
W3C 为我们制定了 DOM 标准;
BOM 的标准, 是在 HTML5发布后, 得到了解决;

> 总结

Javascript 是一种专为与网页交互而设计的脚本语言.