---
title: CPP中的字符串变量的sz前缀是什么意思
date: 2025-01-27
author: 火箭
cover: https://cdn.pixabay.com/photo/2023/09/17/14/40/ai-generated-8258728_1280.png 
categories:
  - 技术博客
tags:
  - c++
draft: false
---

<!--more-->
## 背景介绍

在最近参与的一个VNC远程控制项目中，我接触到了UltraVNC的源码。该项目采用了[UltraVNC](https://github.com/ultravnc/UltraVNC)的定制版本作为服务端，配合[Apache Guacamole](https://guacamole.apache.org/)作为客户端，实现了浏览器端的远程桌面控制功能。

## 发现命名惯例

在深入研究UltraVNC源码时，我注意到了一个有趣的命名模式：**几乎所有的字符串变量都以"sz"作为前缀**，例如：

```cpp
char* szCmdLine = szCmdLine2;
```

## "sz"前缀的由来

通过查阅资料，我在[StackExchange](https://softwareengineering.stackexchange.com/questions/450259/why-is-the-term-string-so-often-abbreviated-as-sz)上找到了答案：

"sz"代表"zero-terminated string"（以零结尾的字符串）。这个命名约定源于：
1. C/C++中的字符串默认以空字符'\0'结尾
2. "sz"是"string zero"的缩写
3. 这种命名法属于匈牙利命名法的一种应用

> So many books,so little time
