---
title: 更新日志
date: 2023-09-07 14:00:00
categories: 编程
tags: 日志
---

# 更新日志

## 2023-02-14

- 新增一篇文章《一款轻量级的虚拟机 Multipass》
- 修改deploy部署方式为gitee和github同时上传，由于github受网络影响，可能会出现失败情况。需要多执行几次`hexo d`

## 2023-02-07

- 新增一篇文章

## 2023-02-06

- 找到插入 cover 图片方法
- 新增一篇文章

## 2023-02-03

- 更换主题为 butterfly，设置 cover 封面，图片显示在左边

- 尝试在.md 文件中的图片使用相对路径
  > 例如： image.jpg 位置为 /2020/01/02/foo/image.jpg ，这表示它是 /2020/01/02/foo/ 文章的一张资源图片， ![](image.jpg) 将会被解析为 <img src="/2020/01/02/foo/image.jpg">
  - 根据 hexo 官方文档(https://hexo.io/zh-cn/docs/asset-folders)操作，还没成功。

## 2023-02-02

- 增加 github 仓库
- 增加 github-pages 分支作为 github 发布页
- 增加搜索插件：'npm install hexo-generator-searchdb --save'
