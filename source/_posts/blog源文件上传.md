---

title: 如何上传本地Hexo博客源码至github page的分支上
date: 2020-4-20
tags:
	- hexo
	- git
---

hexo部署网站到github上是只部署.deploy_git中的静态内容的，像source文件夹之类的是不会自动上传的，也就无法在别的电脑上想要对博客进行修改操作，因此，将文件源码进行托管就显得很重要

<!--more-->

## 1.在github上创建一个分支（source），并将其设为默认分支

## 2.随便找一个目录下打开git bash

	git clone https://github.com/Lrinl/Lrinl.github.io.git

## 3.把克隆到本地的文件中的除.git文件外全都删除

- 如果themes里面有.git文件，把那个git文件夹也删除

## 4.把博客源文件都复制过来

- 除了.deploy_git文件夹

## 5.执行下列执行
	git add .
	git commit -m 'blog source'
	git push

---

## 如果想要更换电脑操作

- 安装git,完成初始设置

- 安装node.js

- 利用npm安装cnpm

```
  npm install -g cnpm --registry=http://registry.npm.taobao.org
```

- 安装hexo

```
cnpm install hexo-cli -g
```

- 进入到克隆下来的文件夹里

```
cnpm install
cnpm install hexo-deployer-git --save
```

- 生成和部署

```
hexo g
hexo d
```

---

**记得在写完后把源文件上传**

