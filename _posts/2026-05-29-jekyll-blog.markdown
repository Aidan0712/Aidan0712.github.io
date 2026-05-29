---
layout: post
title:  "创新实验：使用 Jekyll + GitHub Pages 搭建个人博客"
date:   2026-05-29 10:00:00 +0800
categories: 实验记录
---

这是创新实验第13周的 Jekyll 收尾任务，目标是将 Jekyll 项目推送到 GitHub，并通过 GitHub Pages 实现公网访问。

## 实验目标

1. 配置 Jekyll 项目的 GitHub Actions 自动化部署
2. 创建 gh-pages 分支存放编译后的静态文件
3. 实现代码提交后自动构建部署

## 实现步骤

### 1. 配置 GitHub Actions

创建 `.github/workflows/jekyll-gh-pages.yml` 配置文件，实现自动化构建和部署。

### 2. 创建 gh-pages 分支

使用 orphan 分支创建一个干净的分支用于存放编译后的网站文件。

### 3. 配置仓库设置

在 GitHub 仓库设置中指定 Pages 的源为 gh-pages 分支。

## 遇到的问题

在配置过程中遇到了一些问题，主要包括：

- 权限问题导致无法在容器内创建文件
- GitHub Actions 部署路径配置错误
- gh-pages 分支缺少必要的文件

通过逐步排查和调试，最终成功解决了所有问题。

## 总结

通过本次实验，我掌握了：
- Jekyll 项目的 Docker 化开发
- GitHub Actions 自动化部署流程
- GitHub Pages 的配置和使用

这是一个非常有价值的学习经历！
