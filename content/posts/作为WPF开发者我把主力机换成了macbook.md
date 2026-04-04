---
title: "作为WPF开发者，我把主力机换成了MacBook"
date: 2026-03-08T18:45:04+08:00
author: 火箭
categories:
  - 日常分享
tags:
  - MacBook
  - WPF
  - 开发环境
  - 随笔
cover: https://tuchuang-1258410772.cos.ap-guangzhou.myqcloud.com/Gemini_Generated_Image_4quvl74quvl74quv.png
draft: false
slug: "wpf-developer-switched-main-machine-to-macbook"
description: "随着 AI Coding 时代的到来，作为一个 Windows 钉子户、WPF 开发者，我还是把开发主力机从 Windows 换成了 MacBook。"
keywords:
  - MacBook
  - WPF
  - Windows开发
  - 远程开发
  - 开发环境
---

## 最开始买 MacBook，其实就是单纯想买

我第一次买 MacBook，是 2021 年买的 M1 MacBook Air。

那时候我其实还是做 Windows 开发，Mac 对工作并没有什么直接帮助。说白了，当时买它主要就是因为自己买得起了，看 MacBook 看久了有点上头，想体验一下。

不过那台 M1 Air 后来我自己用得并不多。因为工作环境还是 Windows 为主，它很多时候只是家里的一台苹果笔记本。再后来，这台机器基本就被我老婆拿去追剧了。

## 我自己配了台 Windows 台式机
公司发的 Windows 笔记本编译项目太慢了。那时候我们的项目编译一次差不多要两分钟，写客户端的时候，这种等待真的很烦。刚好我也一直想自己组一台台式机，就干脆把这事一起办了。

台式机配好以后，我平时真正写代码、编译项目、调试问题，基本都在这台机器上完成。到这里为止，我的开发环境其实就稳定下来了。平时我就在台式机配上双屏显示器写代码、看文档，开会的时候用公司配的联想 Windows 本。

## AI 把我的工作流也改了

后面 AI 工具起来以后，我自己写代码的方式其实也变了。

最开始我用的是 GitHub Copilot。那时候我的开发模式已经从“自己把函数一点点敲出来”，慢慢变成了“先写注释，再等 Copilot 补全，然后我来调整代码”。那时候我的主力 IDE 还是 Visual Studio 加 ReSharper。

后来 AI 更强了，我又换到了 Agent 模式更猛一点的 Cursor。再往后，我的工作流就变成了 Visual Studio 负责调试，Cursor 负责生成代码。再后来，我干脆把调试环境也配到了 Cursor 里，开始更彻底地拥抱基于 VS Code 的那套插件生态。

这一步对我影响其实挺大的。因为从那个时候开始，我打开 Visual Studio 的次数越来越少了。也是从那个阶段开始，我开始认真折腾“把主力机器换成 MacBook”这件事。当时我先拿自己的 MacBook Air 做实验。

## 为了把这套双机工作流跑顺，我中间折腾过一圈工具

最开始我查到的是 Synergy，这东西可以做两台电脑的键鼠同步，但它是商业软件，我不想付费。

后面我又去试了 Synergy 的开源版本 Barrier。能用是能用，但稳定性不太行，有时候会卡住。

再后来我还试过 Parsec。它号称可以远程打游戏，按理说延迟应该不是问题，但我用它滑动滚轮看代码的时候，代码会出现一种从模糊到清晰的变化。能用是能用，但体验不太好。

再后来我又试了网易 UU 远程，这个效果已经很好了。我其实用它用了挺长时间，直到后来我发现可以直接用 RDP 协议。

最后我才把现在这套方案跑顺：MacBook 外接显示器，然后通过 RDP 去控制工位上的 Windows 台式机，鼠标和键盘都连接在 MacBook 上。这个方案对我来说几乎没什么延迟，也是我目前用过最舒服的双机方案。

## 后来我向公司申请了一台 MacBook Pro

当我把这套工作流验证得差不多以后，我就把公司配的 Windows 本换成了 MacBook Pro。换机过程还比较有趣。我问了行政同学，他说可以把 Windows 本换成 MacBook，但现在库存里只有 Intel 芯片的机器。我就没换，说等有了 M 芯片的机器再喊我一声。没过多久，行政同学说有了 M5 芯片的 MacBook Pro，可以申请了，我立马就申请了。不得不说，M5 的 MacBook Pro 是真香。

## MacBook 非常适合探索 AI 相关的技术
基于 MacBook 类 Unix 的设计，它确实非常适合探索一些新的 AI 技术栈。有时候我在 Windows 上光是配环境就要花很长时间，但在 Mac 上可能只要几行命令，我就可以把服务跑起来。因为现在做的是 AI 相关的项目，很少写 WPF 相关的代码了，所以我用 MacBook 也越来越顺手了。尤其是 MacBook 的显示屏，看着确实很舒服。

## 双机的痛点
1. Command 键、Option 键和 Windows 上 Alt、Win 键的映射关系会让人分裂。
2. macOS 的很多设计和 Windows 不一样，需要一个适应的过程。

