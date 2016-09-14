---
layout: post
title: PHP操作Session的原理及提升安全性时的一个问题
category: 技术
tags: PHP
description: PHP操作Session的原理及提升安全性时的一个问题
---

昨天在烽火面试，被问到一个很基础的布局问题（一个容器下三个div，两边固定中间自适应）

面试官说我笔试的时候写错了，说实话当时有点蒙，他当时问我再回答一下，结果我蒙的不行又回答了一次，结果听面试官意思应该还是不行

回来之后很气啊，就自己实现一遍，最后发现我确实不对。。。

回来之后实现代码如下；

```html
        <div id="left"></div>
        <div id="right"></div>
        <div id="main"></div>
        html,body {
            margin:0;
            padding:0;
            height: 100%;
            }

            #left,
            #right {
            position: absolute;
            top:0;
            width: 220px;
            height: 100%;
            background:linear-gradient(136deg, #84C5BF, #309E85);
            }

            #left {
            left:0;
            }

            #right {
            right:0;
            }

            #main {
                background: linear-gradient(136deg, #C584AB, #309E85);
            margin: 0 230px;
            height: 100%;
        }
```
