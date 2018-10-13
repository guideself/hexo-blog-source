---
title: 基于Hexo的博客系统
date: 2018-07-04 20:43:43
categories: 'Hexo系列'

---
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;借用官方的说法，[Hexo](https://hexo.io/zh-cn/docs/index.html) 是一个快速、简洁且高效的博客框架。Hexo 使用 Markdown（或其他渲染引擎）解析文章，在几秒内，即可利用靓丽的主题生成静态网页。我借助于该网站按步骤搭建了现在你们看到的这个博客系统，以后我们写好的博客可以直接发布到这个系统上面去，简单自由，不用受制于其他第三方博客网站的约束。
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;下面我将搭建的过程简单记录备用。

## 开始

### 安装软件 Git、Node.js
需要安装的软件有：Git、Node.js，我使用的是windos系统，所以这2个软件下载对应windows版本的软件就可以了，然后依次安装。

### 安装Hexo
1、在本地磁盘中建立一个文件夹，并cd到该目录，我选的是E:\blog<br>
2、安装hexo命令：npm i -g hexo<br>
3、初始化命令：hexo init，执行完成之后，会在该目录下生成很多文件
![](https://i.imgur.com/3MoYLoC.png)

### github上注册账号，创建仓库
这里需要注意repository name命名xxxxx.github.io

### 配置参数，编辑_config.yml
1、本地启动参数<br>
![](https://i.imgur.com/w9cXZpO.png)

2、部署到github参数：<br>
![](https://i.imgur.com/lQBtacI.png)

### 启动和发布
1、本地预览启动
```
hexo clean 
```

```
hexo generate
```

```
hexo server
```


![](https://i.imgur.com/9EVnbI7.png)


2、发布到github

```
hexo clean
```

```
hexo generate
```

```
hexo deploy
```

![](https://i.imgur.com/mK4PW6Q.png)



### 结尾
以上就是我参考网上的资料，逐渐搭建完成的步骤，大概的步骤就是这样子的，最初的系统肯定很简陋，后续可以上网查找资料完善系统其它配置，比如主题，百度统计、评论等等，所以想着之后再写一篇来记录这个过程。