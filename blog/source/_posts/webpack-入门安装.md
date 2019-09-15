---
title: webpack-入门安装
date: 2019-09-11 12:03:24
tags:
  - 前端
  - webpack打包
---
## webpack
### webpack安装
##### webpack是一个前端打包工具。一些 js 资源彼此之前存在依赖关系，当一个页面需要加载多个 .js 的话，也会拖累整个页面的加载速度。所以为了解决这个问题， 如图所示，webpack 就把左边的各种各样的静态资源，打包成了一个所谓的 assets. 这样浏览器加载起来就快多了。


![效果图](http://stepimagewm.how2j.cn/7949.png)

<!--more-->

### node.js
##### webpack 的运行，是需要依赖 node.js 的运行环境的，所以请安装 node.js。

### 关于webpack版本
##### 在 windows 里安装， 用 cnpm 方式安装 @1.13.2 版本是可以正常运行的。

### 安装webpack
##### cmd中指令：cnpm install -g webpack@1.13.2 
##### 安装结束后，运行：webpack，效果如图：
![效果图](http://stepimagewm.how2j.cn/7953.png)
