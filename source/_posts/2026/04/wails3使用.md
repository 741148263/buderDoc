---
title: wails3使用
tags:
  - go
  - wails3
  - vue
  - typescript
categories:
  - go
toc: true
recommend: 1
keywords: categories-go
uniqueId: 2026-04-29 15:27:14/wails3使用.html
mathJax: false
date: 2026-04-29 23:27:14
thumbnail:
---
> 摘要
使用go语言结合wail3开发框架开发桌面应用程序app


# wails3使用


## wails3安装

## wails运行

[踩坑记录]

1. 使用`wails3 dev`运行时提示连接localhost对应的端口失败

![运行ipv6优先级高导致使用端口失败](https://raw.githubusercontent.com/741148263/MyPicBed/main/typora/20260429233025702.png)

**解决办法**[设置IPV4优先](https://blog.xiaoz.org/archives/20079)

```txt
# 查询优先级
netsh interface ipv6 show prefixpolicies
# 在管理员终端中提高ipv4优先级
netsh interface ipv6 set prefixpolicy ::ffff:0:0/96 100 4
```

![](https://raw.githubusercontent.com/741148263/MyPicBed/main/typora/20260429233359292.png)