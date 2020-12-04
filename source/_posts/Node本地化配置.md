---
title: Node本地化配置
date: 2020-11-22 01:04:22
updated: 2020-11-22 01:04:22
tags: 'Nodejs'
categories: '笔记'
comments: true
---

## node 环境配置

- 新增环境变量 NODE_HOME

  - 值为 D:\nodejs

    注：此处可自行设定

- 修改 Path

  - 追加 %NODE_HOME%\
  - 追加 %NODE_HOME%\node_modules\
  - 追加 %NODE_HOME%\node_modules\npm\node_global_modules\



## node 配置

```cmd
cmd /c npm config set prefix "%NODE_HOME%\node_modules\npm\node_global_modules"
cmd /c npm config set cache "%NODE_HOME%\node_modules\npm\node_cache"
cmd /c npm config set registry https://registry.npm.taobao.org
exit
```


