+++
title = 'Devsidecar：解决Github访问慢的问题'
date = 2025-02-17T16:34:01+08:00
categories = '技术'
tags = ['Github']
+++

# 介绍
在国内访问Github的时候，经常会遇到超时或者无法连接的问题，
该如何在不搭梯子（VPN）的前提下解决这个问题呢？
## 原因
> 我们在访问 GitHub 官网时，若是直接访问域名（github.com），则中间有个域名需要通过 DNS 解析的过程被解析为对应的 IP 地址，其实主要时间都是花在了 DNS 解析上，导致了 GitHub 官网有时候能打开，有时候打不开，有时候访问很慢。
# 解决办法
网上有很多手动修改Hosts文件的办法，我觉得还是过于繁琐，这里给大家推荐几个工具

## Devsidecar
这是[wnagliang](https://github.com/wangliang181230)大佬的作品[Devsidecar](https://github.com/docmirror/dev-sidecar)，非常实用，这里引用一段github的介绍
>开发者边车，命名取自service-mesh的service-sidecar，意为为开发者打辅助的边车工具（以下简称ds） 通过本地代理的方式将https请求代理到一些国内的加速通道上

具体可以到[Github仓库](https://github.com/docmirror/dev-sidecar)上看详细的介绍

工具托管在Github上，这里也放一份加速下载的连接：

https://wwpt.lanzoul.com/iOIbJ2o3hbpi
密码: xnz123
## Github520 + SwitchHosts
这个方案也是Hosts修改，但是用了SwitchHosts工具作修改，省去了手动修改的麻烦，还能同步网上的hosts文件
### SwitchHosts
[SwitchHosts](https://github.com/oldj/SwitchHosts/blob/master/README.zh_hans.md)

SwitchHosts 是一个管理 hosts 文件的应用快速切换 hosts 方案  
有许多优点
>- hosts 语法高亮
>- 支持从网络加载远程 hosts 配置
>- 可从系统菜单栏图标快速切换 hosts
这里也提供一个[Gihtub520](https://github.com/521xueweihan/GitHub520)提供的Hosts链接
[Hosts链接](https://raw.hellogithub.com/hosts)
