---
title: python的uv管理器
date: 2026-04-26 20:14:16
tags: python
---

# uv简要说明

> `python`包和项目管理工具

## 一、uv的安装

1. 直接从[github Release](https://github.com/astral-sh/uv/releases)下载发布文件
2. `uv`升级, 使用升级命令`uv self update`


## uv的基础使用命令

|操作|指令|备注|
|:---:|:---|:---|
|安装特定版本|`uv python install 3.12`||
|安装多个版本|`uv python install 3.11 3.12`||
|创建虚拟环境|`uv venv --python 3.11.6`|创建3.11.6版本的虚拟环境，如果该版本不存在，那么会先下载安装后创建虚拟环境|
|查看已安装和可用python版本|`uv python list`||
|筛选指定版本|`uv python list 3.13`|筛选出python3.13的解释器版本|   


