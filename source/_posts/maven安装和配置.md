---
title: maven安装和配置
date: 2018-07-22 16:33:40
categories: 'maven指南'

---
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;借用官方的说法，[Maven](http://maven.apache.org/) 概括地说，Maven简化和标准化项目建设过程。处理编译，分配，文档，团队协作和其他任务的无缝连接。 Maven增加可重用性并负责建立相关的任务。我借助于该网站学习到了maven，现在记录这个学习的过程与大家分享。

## 开始

### maven安装
安装环境说明：Maven3.3以上需要JDK1.7以上<br>
1、下载安装jdk并配置好环境变量，这一步这里不做介绍<br>
2、下载安装并配置maven3.5.4,下载地址：[http://maven.apache.org/download.cgi](http://maven.apache.org/download.cgi "下载地址")
![](https://i.imgur.com/jeNxV4G.png)
解压下载好的maven压缩包到任意目录
配置系统变量
![](https://i.imgur.com/yIj8bkf.png)
![](https://i.imgur.com/KBykdfW.png)
验证是否按照成功
以管理员身份运行cmd，输入命令，如果出现下面信息说明按照成功
![](https://i.imgur.com/e7dt4ym.png)
修改maven默认仓库为阿里仓库
修改为国内仓库后，以后下载jar包会很快
![](https://i.imgur.com/2Im0Dh3.png)

Eclipse中添加安装好的maven
![](https://i.imgur.com/q1QHIHk.png)


### 使用命令创建maven工程
1、在任意目录下建立一个文件夹，用来存放工程<br>
2、使用cmd管理员身份运行，进入
![](https://i.imgur.com/zmgKiLO.png)
最后一条命令：
mvn archetype:generate -DgroupId=com.mycompany.app -DartifactId=my-app -DarchetypeArtifactId=maven-archetype-quickstart -DinteractiveMode=false
是会在选定的目录下创建一个my-app的maven项目，这个过程会下载需要的依赖文件。
执行完毕后，出现下面提示：
![](https://i.imgur.com/1pElvuz.png)

将生产的项目导入到eclipse，用来查看下项目的目录结构：
![](https://i.imgur.com/wvFdwto.png)

重新回到cmd命令窗口，打包应用
![](https://i.imgur.com/ltF6ce4.png)
![](https://i.imgur.com/XINMc7d.png)

可以看到，打包成功后在对应目录下生成了jar文件my-app-1.0-SNAPSHOT.jar
这里我们来运行这个项目，执行下面的命令；
命令由依赖的jar文件和程序的入库类组成
![](https://i.imgur.com/ZOjz0eb.png)

其他maven命令，可以查询官方手册了解：
![](https://i.imgur.com/tJqy8AR.png)



### 结尾
安装maven的过程还是很清晰的，没有特别注意的关注点，按照步骤完成即可，接下来的内容就是逐步深入了解maven了，我还是倾向于依照官方网站指引来学习。