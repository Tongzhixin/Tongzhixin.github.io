---
title: ssh_tutorial
abbrlink: 11713
date: 2019-07-17 21:47:51
tags: ssh
---
### vscode远程控制的准备

#### 简介：刚开始使用ssh密钥时的踩坑记录

 在网站上下载[openssh/（win10/）](https://www.mls-software.com/opensshd.html,"下载来源")，至于与putty和git生成的密钥，网上一致的声音是，openssh暂时没有后两者好用，但是当我把坑踩了好多之后，明白了ssh的道理之后就感觉几种之间并没有太大的区别，因为都是用的ssh机制，只不过是一种验证工具。下面是我总结的一点语句：
 首先我们要清楚ssh密钥和配置都在`C:\Users\名字\.ssh`中，名字有几种，分别为`id_rsa`等`ssh-keygen -t rsa -C who@where、scp`，我突然看到一篇[博客](https://qidawu.github.io/2016/10/06/ssh/)，很🆗，另外一个使[vscode连接远程操控的方式](https://blog.csdn.net/lenfranky/article/details/89972889)
 [这个](https://blog.csdn.net/maguanzhan7939/article/details/94398745)也可以。