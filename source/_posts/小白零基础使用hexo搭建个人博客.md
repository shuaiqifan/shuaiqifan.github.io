---
title: 小白零基础使用hexo搭建个人博客
date: 2021-10-27 12:51:57
categories:
- hexo
tags: 
- 搭建个人博客
- hexo
---

# 从零开始搭建个人博客



## 目录



---

## 安装实操

### 1.下载 并安装 Node.js

[Node.js](https://nodejs.org/zh-cn/)的官方网址，下载长期维护版

安装完成以后，输入`node -v`和`npm -v`通过查看安装的Node.js版本来测试安装是否成功

### 2.下载Git

[Git官网](https://git-scm.com/)，在右侧小电脑那点击`Download for windows`

安装好后，用`git --version` 来查看一下版本

### 3.安装Hexo框架

```
npm install hexo-cli -g 
```

通过输入`hexo -v`来验证Hexo是否安装成功

在管理员命令窗口使用`cd`命令切换到系统盘之外的其他盘,输入下面指令新建一个blog文件夹

```
hexo init blog
```

切换到blog文件夹

```
cd blog
```

安装依赖包

```
npm install
```

启动Hexo网址 `http://localhost:4000/`

```
hexo server
```

至此，Hexo个人博客基本框架就安装完毕了，是不是超级简单呢。

---

你以为到此就完结了吗，NONONO，我们还需要进行个性化配置

## 个性化配置博客

把博客生成Public静态文件夹,生成好的Public文件夹可以直接当成静态网站进行部署

``` 
hexo g
```

### 1.更换Hexo主题

打开[Hexo官网主题页](https://hexo.io/themes/)，在里面挑选一款自己喜欢的博客主题，点击进去之后，主题博主会告诉你怎么安装他开发的主题。下面我将以我自己的主题为例，分享一下该怎么更换自己喜欢的主题，使自己的主题页面看起来更加美观酷炫。

1.在以管理员身份打开的Windows命令控制行中，使用`cd`命令切换到`blog`文件夹，输入命令

```
git clone -b master https://github.com/jerryc127/hexo-theme-butterfly.git themes/butterfly
```

2.使用VS Code编辑器打开blog文件夹，打开`_config.yml`文件并修改`theme`

```
theme: butterfly
```

3.如果你的主题需要安装插件，提示如果没有pug以及stylus的渲染器，使用`npm`指令安装一下

```
npm install hexo-renderer-pug hexo-renderer-stylus --save
```



## Hexo常用指令

创建文章

```
hexo n "文章名"
```







