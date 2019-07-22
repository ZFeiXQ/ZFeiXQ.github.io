---
layout: post
title: "obfuscation"
description: "os"
category: 学习技术
tags: [基础知识]
---
{% include JB/setup %}
##obfuscation

前几天去听了几天的培训，晕晕乎乎，深刻的明白英语的重要性，，，故决定看看ppt

第二天。。。

介绍混淆

提出man-at-the-end（MATE）：个人理解可以成为白盒攻击，首先攻击者是人，他们拥有一定的智慧和能力，同时也可能拥有和正常用户一样的访问硬件护或者软件的权限，通过一定的技术手段（逆向，调试等）篡改或者调试硬件或软件本身，常见的保护方法有混淆，水印的 等！

英文定义：
Man-At-The-End (MATE) attacks occur in any setting where an adversary has physical access to a
device and compromises it by inspecting, reverse engineering, or tampering with its hardware or
software.

Remote Man-At-The-End (R-MATE) attacks occur in distributed systems where untrusted clients
communicate with trusted servers, and malicious users get an advantage by compromising an untrusted device.

代码转换：是对程序进行改变，为了让代码的行为或者语义相同，但是改变的代码在一定程度上更好！（更好是指faster,smaller,more security）

A code transformation takes a program and changes it so that it behaves the same (its semantics
doesn't change), but it is “better” in some way.

编译器可以让程序变得更快：

1.过程内联用替换成一个函数调用！（内联函数是指在程序中频繁调用某个函数时会产生入栈操作实现栈内空间增大，加入inline，使得程序在运行时直接调用函数体内的代码，从而能提高效率）

2.复制循环体，用循环展开来替换循环

##混淆的目标：

1，让人很难理解
2.很难采用逆向工程等工具自动化分析
隐藏程序中的许多资产

##混淆的步骤：
![](/assets/img/obfuscation/obufucation.png)

##

## 参考
https://blog.csdn.net/zqixiao_09/article/details/50877383