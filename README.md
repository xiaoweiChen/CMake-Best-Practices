# CMake Best Practices

*Discover proven techniques for creating and maintaining programming projects with CMake *

*(使用CMake创建和维护项目)*

<a><img src="cover.jpg" height="256px" align="right"></a>

* 作者：Dominik Berner, Mustafa Kemal Gilor  
* 译者：陈晓伟
* 首次发布时间：2022年5月27日([来源](https://www.amazon.com/dp/1803239727))

> 翻译是译者用自己的思想，换一种语言，对原作者想法的重新阐释。鉴于我的学识所限，误解和错译在所难免。如果你能买到本书的原版，且有能力阅读英文，请直接去读原文。因为与之相较，我的译文可能根本不值得一读。
>
> <p align="right"> — 云风，程序员修炼之道第2版译者</p>

PDF可在本库的[Release页面](https://github.com/xiaoweiChen/CMake-Best-Practices/releases)获取。

## 本书概述

CMake是一个强大的工具，用于执行各种各样的任务，所以很难找到一个起点进行学习CMake。这本书更专注于了最常见的任务，边实践边学习CMake。CMake文档很全面，但缺少具有代表性的例子，说明如何将源码组合在一起，特别是互联网上还有有很奇淫技巧和过时的解决方案。本书的重点是帮助读者把需要做的事情串在一起，编写CMake，从而创建简洁和可维护的项目。

阅读本书后，不仅可以掌握CMake的基础知识，而且还可以通过构建大型复杂项目和创建在任何编程环境中运行的构建示例。还可以使用集成和自动化的各种工具，以提高整体软件质量的方法，例如：测试框架、模糊测试器和自动生成文档。编写代码只是工作的一半，本书还会引导读者对程序进行安装、打包和分发，这些都是为使用CI/CD的现代开发工作流程需要的基础功能。

读完这本书，将能以最好的方式使用CMake建立和维护复杂的软件项目。

#### 关键特性

- 理解CMake是什么，如何工作，如何与其交互
- 了解如何正确地创建和维护结构良好的CMake项目
- 探索工具和技术，以最大程度的使用CMake管理项目

#### 将会学到

- 构建结构良好的CMake项目

- 跨项目模块化和重用CMake代码

- 将各种静态分析、检测、格式化和文档生成工具集成到CMake项目中

- 尝试进行跨平台构建

- 了解如何使用不同的工具链

- 为项目构建一个定义良好，且可移植的构建环境

  

## 适读人群

这本书针对软件工程师和构建系统维护人员，他们经常使用C或C++，使用CMake可以更好地完成他们的日常任务。对C++和一般编程知识有所了解的话，会有助于您更好地理解书中的例子。

## 作者简介

**Dominik Berner**是一位拥有20年专业软件开发经验的软件工程师、博客作者和演讲者。主要使用C++，还参与了许多软件项目，从为初创公司的外科手术模拟器编写前沿软件，到为MedTech行业的大型企业维护大型平台，再到为介于两者之间的公司创建物联网解决方案。他相信，良好设计和维护的构建环境是使团队高效编写软件，并创建高质量软件的关键因素之一。当他不写代码的时候，偶尔会去博客写一些文章，或者在会议上发表一些关于软件开发的演讲。

> "我想感谢为本书做出贡献的人们:合著者Mustafa Gilor，他补充了我的专业知识；Kinnari Chohan是一个出色的编辑；Gebin George启动了这本书，以及Packt的整个团队。非常感谢我们的技术评审，Richard von Lehe, Horváth V.和Toni Solarin-Sodara。最后，感谢我的家人，Brigitte、Alice和Theo，在我写这本书的时候给予我耐心和支持!"  
>
> <p align="right"> —Dominik Berner</p>

**Mustafa Kemal Gilor**是一位经验丰富的专业人员，从事电信、国防工业和开源软件的性能关键软件开发。他的专长是高性能和可扩展的软件设计、网络技术、DevOps和软件架构。他对计算机的兴趣在童年时期就显现出来了。他在12岁左右学习编程破解MMORPG游戏，从那时起他就一直在编写软件。他最喜欢的编程语言是C++，并且喜欢做框架设计和系统编程，也是CMake的坚定倡导者。他的职业生涯中，维护了许多代码库，并将许多遗留(非CMamek)项目移植到CMake。

> "首先，我要感谢我的合著者，Packt Publishing的Dominik Berner，以及所有用他们宝贵的工作使这本书成为可能的技术审评。我还要感谢我生命中最善良、最理解我的人——我的妻子Büşra，在写作的过程中，她给了我所需要的支持和鼓励。最后，我要感谢家人和朋友Gürcan Pehlevan, Ramazan Cömert, Mustafa Hergül, Habip İşler，以及Ahmet Aksoy，感谢他们在整个过程中对我的信任和支持。"  
>
> <p align="right"> —Mustafa Kemal Gilor </p>



## 审评者介绍

**Richard Von Lehe** 住在明尼苏达州的双城地区。过去的几年中，他在软件项目中经常使用CMake，包括正畸建模、建筑控制、无人机避免碰撞和专用打印机。闲暇时，他喜欢和家人以及他们的宠物兔子Gus一起放松。他还喜欢骑自行车和弹吉他。

**Toni Solarin-Solada** 是一名软件工程师，专门设计抽象底层操作系统服务的跨平台编程库。

## 本书相关

* github地址：https://github.com/xiaoweiChen/CMake-Best-Practices
* 译文的LaTeX 环境配置：https://www.cnblogs.com/1625--H/p/11524968.html 
  * 禁用拼写检查：https://blog.csdn.net/weixin_39278265/article/details/87931348

* vscode中配置latex：https://blog.csdn.net/Ruins_LEE/article/details/123555016
* 原书示例：https://github.com/PacktPublishing/CMake-Best-Practices

