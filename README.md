# myblog
GitHub博客创建
##1.详细操作过程
操作步骤：

在 GitHub 上创建一个新的仓库：

登录到 GitHub。

点击右上角的 +，选择 New repository。

填写仓库的名称，比如 my-blog。

选择 Public（公开），勾选 Initialize this repository with a README。

点击 Create repository。

##2.本机操作或GitHub上操作要明确说明
2. 设置 GitHub Pages
启用 GitHub Pages：

进入你的仓库页面，点击 Settings。

滚动到 GitHub Pages 部分。

在 Source 部分，选择 main 或 master 分支，然后选择 / (root)。

点击 Save。你将看到一个网址，表示 GitHub Pages 已成功启用。

##3.博客如何使用模块？
3. 安装 Jekyll（本地环境）
Jekyll 是一个静态网站生成器，可以帮助你快速创建一个博客。

安装 Ruby 和 Jekyll（本地操作）：

安装 Ruby：

在 Ruby 官网 下载并安装 Ruby。

使用 ruby -v 确认是否安装成功。

安装 Jekyll：
在命令行（终端）中运行以下命令：
gem install jekyll bundler  
创建新的 Jekyll 博客：
在你希望创建博客的文件夹中，运行以下命令：
jekyll new my-blog
cd my-blog
4. 将博客内容推送到 GitHub
进入你本地博客项目的文件夹。

初始化 Git 仓库：
git init
git add .
git commit -m "Initial commit"
连接 GitHub 仓库：
git remote add origin https://github.com/yourusername/my-blog.git
推送内容：
git push -u origin master
5. 博客的配置与模块
修改 _config.yml 配置文件：
在 _config.yml 文件中，你可以修改博客的基本设置，如标题、作者、语言等。例如：
title: My Awesome Blog
author: Ritak
description: "A blog about technology and coding."
theme: minima
使用 Jekyll 模块：
Jekyll 提供了许多内置的模块，可以帮助你更轻松地创建博客。常见的模块包括：

_posts：用于存储博客文章。

_layouts：定义不同页面的布局。

_includes：可重用的 HTML 片段。

_data：可以存储自定义数据。

_assets：静态资源（如图片、CSS、JS）的位置。
6. 本地运行博客
在本地查看博客的效果，可以运行以下命令：
bundle exec jekyll serve
然后打开浏览器并访问 http://localhost:4000 查看博客。

7. 更新博客内容
新建文章：
在 _posts 文件夹中创建新文章。例如，创建一个名为 2025-07-01-my-first-post.md 的 Markdown 文件，内容如下：
---
layout: post
title: "My First Post"
date: 2025-07-01
---
This is my first post on my new blog!
推送更新：

git add .

git commit -m "Add new post"

git push
8. 博客的模块化管理
Jekyll 模块化的管理方式使得你可以非常灵活地定制博客的布局和功能。例如：

使用 _layouts 自定义页面布局：
在 _layouts 文件夹中创建自定义的 HTML 模板，如 default.html、post.html 等。

自定义博客主题：
Jekyll 支持各种主题，你可以通过更改 _config.yml 中的 theme 配置来选择其他主题，或者开发自己的主题。
总结：
创建 GitHub 仓库并启用 GitHub Pages。

安装并使用 Jekyll 来生成博客。

配置和模块化管理博客，使用 _posts、_layouts 等文件夹来存储和管理内容。
