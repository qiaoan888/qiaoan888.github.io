---
layout: post
title: Build a blog
---
如何利用jekyll和Github 搭建博客？
# 目录
+ [注册Github](#partI)
+ [创建仓库](#partII)
+ [开启Github Pages](#partIII)
+ [安装Ruby](#partIV)
+ [安装Jekyll](#partV)
+ [创建博客](#partVI)
+ [复制主题](#partVII)


## 注册Github <p id="partI"></p>
1、当我们进入官网后会出现登陆的界面
（1）是输入用户、邮箱、密码的地方。（2）是当你注册好了之后或者已注册之后点击这里跳转到登陆的界面。
（3）是当你第一次使用还没有账号的情况，点击这里进行注册。（4）是登陆GitHub。如果你已经有账号了则直接点击sign in 去登陆就可以了。

2、点击sign up之后出现的这个页面
（1）页面中第一个输入栏输入用户名、第二栏输入你邮箱地址，GitHub是通过邮箱激活方式来注册的。
（2）全部输入完成之后点击页面底部的create an account 创建账号 （3）继续下一步是激活邮箱激活,之后就注册成功了。



## 创建仓库 <p id="partII"></p>
在Github首页右上角头像左侧加号点选择 New repositor(新存储库)进行创建一个仓库.



## 开启Github Pages <p id="partIII"></p>


当你的仓库名为：用户名.github.io 之后默认开启Github Pages

3.现在随便选择一个主题,选择上图的 Choose a theme 之后会跳转到下面这个页面


设置完毕后你就可以通过（ https://你的用户名.github.io ）进行博客访问


## 安装Ruby <p id="partIV"></p>
Windows 用户访问 http://rubyinstaller.org/ 下载 130.9MB  大小的 rubyinstaller-devkit-2.7.1-1-x64.exe

安装时注意勾选 Add Ruby executables to your PATH，没选的话可以手工配置一下 Path=D:\Develop\Ruby27-x64\bin;...

安装完成后，按照提示再安装 MSYS2（在弹出的窗口选择 3 - MSYS2 and MINGW development toolchain）（这个耗时有点长，慢慢等待…）

然后在命令提示符中验证一下安装结果

![图]({{ site.url }}/assets/YU07(B_(L9_)L%4PF87Q}DX.jpg)

## 安装Jekyll <p id="partV"></p>
这里通过 RubyGems 安装 Jekyll，所以先到官网 https://rubygems.org/ 下载 1.27MB 大小的rubygems-3.1.4.zip

接着解压压缩包到桌面，并在命令提示符中执行安装命令

![图]({{ site.url }}/assets/(LD19IZP%_9{IAF$@4%QH9Q.jpg)

然后删掉 rubygems-3.1.4 文件夹，它没用了

下面进入正题：用 RubyGems 来安装 Jekyll（这个耗时也有点长…）

![图]({{ site.url }}/assets/C9{`J@@)7_IOHTX}@[8OG1N.jpg)

至此，Jekyll就安装完毕了

## 创建博客 <p id="partVI"></p>
先建一个文件夹（这里命名为 Jekyll）用于存放博客内容，然后在命令提示符中执行以下命令创建 Jekyll 工作区

![图]({{ site.url }}/assets/_184PZCNRU14J_IKV[QS0V2.jpg)

注①：在执行完命令后，若过了一段时间控制台还是没有动静，不妨敲一下回车（堵了，执行结果没有输出在控制台上）

注②：以前的 Jekyll 版本曾遇到下面的错误提示，此时需安装 bundler，然后再重新执行命令（记得先删掉上面 new 的 myblog 目录）

![图]({{ site.url }}/assets/WP7`TOT)IRCR43{8DZ(PE33.jpg)

创建完毕，我们回到本地目录看一下

![图]({{ site.url }}/assets/光效.jpg)

接下来到博客文件夹中，启动Jekyll服务

![图]({{ site.url }}/assets/光效.jpg)

访问 http://127.0.0.1:4000/ 会看到下面的页面

![图]({{ site.url }}/assets/光效.![图]({{ site.url }}/assets/光效.jpg)


## 复制主题 <p id="partVII"></p>
这里将该主题代码弄下来后，通过 jekyll s 命令启动来查看本地效果

本地启动时，可能会报告下面的错误

![图]({{ site.url }}/assets/光效.![图]({{ site.url }}/assets/光效.jpg)

这是因为 Jekyll 中默认安装已没有此分页组件，官方将其插件化了，需进行下面操作

![图]({{ site.url }}/assets/光效.jpg)

接着再启动就成功了，访问 http://127.0.0.1:4000/ 就看到本地页面了



