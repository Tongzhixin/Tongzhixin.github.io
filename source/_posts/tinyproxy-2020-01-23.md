---
title: tinyproxy
abbrlink: 25500
date: 2020-01-23 00:23:44
tags: proxy
---
#### tinyproxy使用

首先我们要明确一个概念，代理服务器跟用来fq的服务器比如vps有一点是不一样的。你跟代理服务器之间通信是可以被截取的，而一般fq用的，在你主机与服务器之间会有加密。

tinyproxy就是一款轻量型的http代理服务器，用来爬虫还好。

`apt-get install tinyproxy`

`service tinyproxy start/restart/stop`

`/etc/tinyproxy.conf`

- 端口要改
- Allow要改
- 密码，随便吧