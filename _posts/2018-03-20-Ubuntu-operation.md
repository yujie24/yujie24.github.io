---
layout: post
title: ubuntu简单的一些操作
categories: [技术文档]
description: 收集一些简单的操作口令
keywords: ubuntu, 操作系统
---

## 关机命令

|命令           |作用     |
|------|------|
|halt           |立刻关机|
|poweroff       |立刻关机|
|shutdown -h now|立刻关机（root用户）|
|shutdown -h 10 |10分钟后关机（root用户）|

- 如果用shutdown命令设置关机的话，可用shutdown -c命令取消重启。


## 重启命令

|命令           |作用     |
|------|------|
|reboot           |重启|
|shutdown -r now  |立刻重启（root用户）|
|shutdown -r 10   |过10分钟重启（root用户）|
|shutdown -r 20:00|在20:00时间点重启（root用户）|

- 如果用shutdown命令设置重启的话，可用shutdown -c命令取消重启。


## 重启网卡

|命令           |作用     |
|------|------|
|ifconfig                                        |查看网卡信息|
|ifconfig eth1 192.168.1.10 netmask 255.255.255.0|设定一个网卡IP|
|sudo /etc/init.d/networking restart             |重启网卡使设定生效|
|ifdown eth0                                     |关闭网卡|
|ifup eth0                                       |开启网卡|

- 用ubuntu的系统———>系统管理———>网络设置
- 重启网卡，优点是可以指定网卡，不影响其他网络接口。



## 参考资料：
*（感谢大牛们的总结，让我可以站在巨人的肩膀上）*
- http://blog.csdn.net/babydavic/article/details/21231679
