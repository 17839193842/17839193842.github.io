---
title: hexo & github 搭建个人博客
---
welcome to my blog,this is my first article.  其实,在17年的2月我的博客就已经建立了，上面有好多文章，以及我的经典收藏于一些小经验，放在了一个朋友的子域名下,自从出来实习了，一直没理睬我的博客，昨天打开一看,网址已经打不开了，心情别提多糟了，很无奈，只能用hexo+github重新搭建博客了。。。
## 安装node.js
Node 下载地址: https://nodejs.org/en/
## 安装git
Git下载地址： https://git-for-windows.github.io/
## 安装hexo
``` bash
$ npm install -g hexo
```
## 初始化Hexo
### 创建文件夹
### 在文件夹下右键->Git Bash
``` bash
$ hexo init
```
## 在_config.yml,进行基础配置
    # Site
     title: 博客名字
	 subtitle: 子标题
	 descript: 
	 author: 作者
	 theme: 主题
### 输入命令,获得更多主题
``` bash
$ git clone https://github.com/iissnan/hexo-theme-nextthemes/nex
```
## 本地浏览博客
### 输入命令
``` bash
$ hexo g
```
``` bash
$ hexo s
```
### 在浏览器中输入: localhost:4000 即可访问
## 写文章
### 在XX:\Hexo\source\_posts文件下，新建.md文件就可以写文章
## 部署到Github上面
### 申请账号->新建仓库(命名:账号.github.io)
### 在_config.yml进行配置
    最下面:
	   deploy:
	     type:空格git
		 repo:空格https://github.com/账号.github.io.git
		 branch:空格master
### 安装hexo-deployer-git --save
``` bash
$ npm install hexo-deployer-git --save
```
### 发布到Github上
#### 输入命令
``` bash
$ hexo clean && hexo g && hexo d
```
#### 若出现 INFO Deploy done :git //发布完成
### 在浏览器输入：https://账号.github.io/
     