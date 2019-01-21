---
layout: post
title: "你好世界!"
tags:
  - read
  - jekyll
hero: https://source.unsplash.com/collection/430471/
overlay: blue
published: true
---

# 今天学习了如何使用 `jekyll`搭建一个博客系统

<!–-break-–>

## 1. 安装ruby,依赖于ruby环境

- brew install ruby [ruby环境下载](https://www.ruby-lang.org/en/downloads/)
- sudo gem install jekyll(安装jekyll)
- sudo gem install jekyll bundler(运行工具)

## 2. 安装不上用这个域名(国内镜像)

- gem sources --add https://gems.ruby-china.org/  --remove https://rubygems.org/

## 3. 创建站点

- jekyll new myblog(名称)

## 4. 安装bundle (一些依赖)

- bundle install

## 5. 访问(本地站点)

- bundle exec jekyll serve 

## 6. 文件配置

1. _config.yml :
    选择配置 :
    title(网站标题)
    email(邮箱)
    descripation(描述)
    baseurl(可以部署二级path)

2. 创建_drafts目录,存放未发布草稿
      _site: 存放源代码
3. jekyll build 在_site中创建静态资源


## 7. 部署域名可访问

1. 创建GitHub仓库 : jinjie-me.github.io (前缀要和GitHub的username一致)

2. rm -rf .git 移除原来的git仓库,_config.yml中去除自带的baseurl

3. git init  / git add . / git commit -m "init"


