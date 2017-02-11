---
layout: post
date: 2016-01-12 09:28
title: conoha vps
---


今天在 [conoha.jp](www.conoha.jp) 上买了一个 vps CentOS环境，准备再玩儿一下nodejs，以下是记录的期间遇到的几个问题


##1. 80端口不能访问

装上nodejs PM2 express 写了个helloworld ，在chrome上用ip访问了一下不能访问，第一想到的是80端口没开

装上python 的 requests包

安装request方法：

```
pip install requests
```
用request 请求了一下本级地址，结果没问题

于是去conoha配置面板看了一下，80端口是开放的。

百思不得其姐

于是乎又看了一下系统版本如下： 

```
➜  sysconfig  cat /etc/redhat-release
CentOS Linux release 7.2.1511 (Core)
```

查了一下CentOS 7.2 系统默认是把防火墙开启的，需要手工开启

```
/sbin/iptables -I INPUT -p tcp --dport 80 -j ACCEPT
```

##1. PM2 

github homepage [pm2](https://github.com/Unitech/pm2)

```
$ pm2 start app.js
``` 

## Hapi

[hapijs](http://hapijs.com/tutorials)

