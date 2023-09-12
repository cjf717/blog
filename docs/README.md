---
title: 使用说明,
date: 2023-09-06 12:00:00,
categories: 编程,
tags: blog
---

# 说明
## 建立目的
这是一个由创梦天空创建的个人博客，主要目的是保存和记录文章，以便日后查阅。

# Hexo Blog 项目工程

## 项目使用

```
# npm install
npm run serve
npm run build
```

## 内容说明

- 注意：使用 git 管理，对上传内容会有和谐风险

## git 相关

### 提交上传

#### gitee 操作

```
git add .
git commit -m "init"
// git remote add origin git@gitee.com:jeff-chan/blog.git
git push -u origin "main"
```

#### githup 操作

```
git add .
git commit -m "增加github仓库"
// git branch -M main
//// git remote add github https://github.com/cjf717/cjf717.github.io.git
// git remote add github git@github.com:cjf717/blog.git
git push -u github main
```

### 分支管理

#### 创建分支

```
git checkout -b init
git push -u origin init
git checkout main
```

#### 合并分支

- 可以使用以下命令将其他分支的代码合并到当前分支：`git merge <branch>`
- 如果想将 A 分支合并到 B 分支，就要先切换到 B 分支，然后执行命令：`git merge A`

### 标签

#### 创建标签

```
# git tag -a <tagname> -m "<message>"
git tag -a v0.1.1 -m "init"
# git push origin --tags
git push origin v0.1.1
```

### 强制拉取并覆盖本地文件

```
git fetch --all
git reset --hard origin/main
git pull origin main
```

### github pages 配置

- github 发布静态网站所在目录只能是根目录或者 docs，要在 hexo 中发布文件夹为 public 作为目录，使用 git subtree 命令。[参考文章](https://blog.csdn.net/mrliucx/article/details/125574957)
  1. 建立新的分支 github-pages。
  2. subtree push 到远程仓库。如果存在多个仓库，需要指定仓库。
  3. 选择 github 发布的分支。

```
git checkout -b github-pages
git subtree push --prefix=public github github-pages
git subtree push --prefix=public origin github-pages
```

## hexo 命令

- 新增文章 `hexo new [layout] <title>`
- 清除缓存 `hexo clean`
- 启动本地服务器预览 `hexo s`
- 生成静态文件 `hexo g`
- 部署网站 `hexo d`

## 相关网站

- [Hexo](http://hexo.io/)
  ### butterfly 主题
  - 主题-[butterfly](https://github.com/jerryc127/hexo-theme-butterfly)
  - [hexo-theme-butterfly 官方文档](https://butterfly.js.org/)
  - [butterfly gitee 官网](https://gitee.com/immyw/hexo-theme-butterfly)
  ### Melody 主题
  - 主题-[Melody](https://github.com/Molunerfinn/hexo-theme-melody)
  - [hexo-theme-matery 官方文档](http://blinkfox.com/)
