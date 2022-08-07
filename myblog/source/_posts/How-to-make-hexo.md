---
title: How to make hexo
date: 2022-07-15 21:50:49
tags:
---
## 1 下载git
[git下载网站](https://git-scm.com) 点击downlode即可下载
## 2 下载node.js
（https://nodejs.org）
## 3 下载hexo
先创建一个文件夹blog再cd到这个文件夹下

初始化`hexo init myblog`

`cd myblog //`进入这个myblog文件夹然后`npm insatll`

指定文件夹会有：node_modules: 依赖包
public：存放生成的页面
scaffolds：生成文章的一些模板
source：用来存放你的文章
themes：主题
_config.yml: 博客的配置文件

`hexo g `然后` hexo server `打开hexo的服务在浏览器输入localhost:4000就可以看到你生成的博客了

## 4 github创建个人仓库

先注册一个github账号会看到New repository创建一个和你用户名相同的仓库后面加.github.io只有这样将来要部署到GitHub page的时候才会被识别也就是xxxx.github.io其中xxx就是你注册GitHub的用户名

## 5 把ssh加入到github

回到git bash：输入`git config --user.name"yourname"`然后输入入`git config --user.email"youremail"`

然后创建ssh 一路回车`：ssh-keygen -t rsa -C"youremail"` 这个时候它会告诉你已经生成了.ssh的文件夹。在你的电脑中找到这个文件夹

## 6 hexo部署到github

打开站点配置文件 _config.ym翻到最下面输入

deploy：
```
  type：git
  
  repo:https://github.com/Yourname/yourgithubname.github.io.git

  branch:master

此时要先安装deploy-git：npm install hexo-deployer-git --save

然后：hexo clean

hexo generate

hexo deploy
```

输入这个网址就能看到你的博客了：http://yourname.github.io
