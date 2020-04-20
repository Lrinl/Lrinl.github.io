---
title: 如何上传本地Hexo博客源码至github page的分支上
date: 2020-4-19
---

<!--more-->

## 1.进入博客源文件夹，调用git工具

## 2.初始化本地项目

- git init

## 3.若出现以下情况

- warning: LF will be replaced by CRLF
  ### 解决方法
- git config core.autocrlf false

## 4.将本地Hexo目录与远程仓库关联

- git remote add origin `https://github.com/Lrinl/Lrinl.github.io.git`

## 5.添加所有文件到暂存区

- git add .

## 6.提交暂存区的文件

- git commit -m '我的提交'

## 7.推送本地分支（master）到远程分支（source）上（没有则自动创建）

- git push origin master:source

