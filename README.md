# 朱昊天的个人博客

基于 [Jekyll](https://jekyllrb.com/) 构建，托管于 [GitHub Pages](https://pages.github.com/)。

在线地址：<https://horacezoe.github.io>

## 本地预览

需要安装 Ruby 环境：

```bash
bundle install
bundle exec jekyll serve
```

然后在浏览器打开 <http://localhost:4000>。

## 发布新文章

在 `_posts/` 目录下创建 Markdown 文件，命名格式为 `YYYY-MM-DD-标题.md`：

```markdown
---
layout: post
title: "文章标题"
date: 2025-01-15
categories: [技术]
tags: [Java, 学习笔记]
excerpt: "文章摘要，显示在首页列表中"
---

正文内容写在这里，支持 **Markdown** 语法。

### 插入图片

将图片放入 `assets/images/` 目录，在正文中引用：

```markdown
![图片描述](/assets/images/your-image.png)
```
```

推送到 GitHub 的 `main` 分支后，GitHub Pages 会自动构建并发布。

## 项目结构

```
├── _config.yml          # 站点配置
├── _data/
│   └── navigation.yml   # 导航菜单
├── _includes/           # 可复用 HTML 片段
├── _layouts/            # 页面布局模板
├── _posts/              # 博客文章（Markdown）
├── assets/
│   ├── css/             # 样式文件
│   └── images/          # 文章图片（在 Markdown 中引用）
├── about.md             # 关于页面
├── songs.md             # 音乐收藏页面
└── index.html           # 首页
```

## 自定义

- 修改站点信息：编辑 `_config.yml`
- 修改导航菜单：编辑 `_data/navigation.yml`
- 修改样式：编辑 `assets/css/main.css`
- 添加新页面：在根目录创建 `.md` 文件并设置 `permalink`
