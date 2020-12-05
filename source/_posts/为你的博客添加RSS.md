---
title: 为你的博客添加RSS
comments: true
date: 2020-11-22 08:47:40
updated: 2020-11-22 08:47:40
tags: ['Nodejs', 'hexo']
categories: '笔记'
---

**配置一个RSS很简单，只需要三步！**

（大象装冰箱要几步？）



## 下载并安装插件

按住shift单击右键，选择“ 在此处打开命令窗口”

```cmd
npm install -g hexo-generator-feed
```

( -g 参数随自身情况而定 )

## 配置插件

  在根目录下的 _config.yml 文件中，添加以下代码 

```config
# 配置 Rss 订阅
Plugins: 
- hexo-generate-feed
```

## 添加 RSS

 在 next (或其他主题) 目录下的 _config.yml 文件中，找到 rss 然后添加以下代码 ，如果没有找到 rss ，直接复制过去就 ok 

```config
rss: /atom.xml
```

## 测试

```cmd
hexo clean
hexo generate
hexo server
```

