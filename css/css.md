---
title: css优化
tags: ['css优化']
category: css优化
date: 2017-02-04 10:08:29
---

## 背景
页面优化是永无止境的，写一篇从css的角度来优化页面，持续记录自己的优化过程。
## 优化方法
1. css层级不要嵌套太深
浏览器在渲染的时候，解析css是从右向左，一层层的去遍历寻找，如果层级太多，必然增加了渲染时间。一般是三层以内（包括三层）。
2. 具体的代码模块（不是通用样式），避免使用元素选择器
* 如1所说，在html中，有很多常用的高频元素，比如，div、p、span、a、ul等，如果最内侧使用了元素选择器，在解析css的时候，浏览器会遍历html中所有的此类元素    
* 需求和代码结构都存在着潜在的变化。

## 参考链接 
1. [没那么难，谈CSS的设计模式](http://div.io/topic/1806)




