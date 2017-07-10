<!-- TOC -->

- [1. Git](#1-git)
    - [1.1. Git 安装](#11-git-安装)
    - [1.2. VScode terminal](#12-vscode-terminal)
    - [1.3. git init](#13-git-init)
    - [1.4. git remote add [origin] [仓库地址]](#14-git-remote-add-origin-仓库地址)
    - [1.5. git add](#15-git-add)
    - [1.6. git commit -m ""](#16-git-commit--m-)
    - [1.7. git reset [版本编号] [--hard]](#17-git-reset-版本编号---hard)
    - [1.8. git pull/git push](#18-git-pullgit-push)
- [2. HTML](#2-html)
    - [2.1. 标签](#21-标签)
    - [2.2. 嵌套](#22-嵌套)
    - [2.3. 注释](#23-注释)
    - [2.4. 属性](#24-属性)
    - [2.5. head部分](#25-head部分)
    - [2.6. src href 寻址方式](#26-src-href-寻址方式)
    - [2.7. 文本标签](#27-文本标签)
- [3. 作业](#3-作业)

<!-- /TOC -->

# 1. Git 

Git/SVN 版本控制系统

Git 分布式版本控制系统  少量程序员
SVN 集中式版本控制系统

## 1.1. Git 安装

    勾选，use Git from window command promt

## 1.2. VScode terminal

    Ctrl + `

## 1.3. git init

    初始化仓库 repo

## 1.4. git remote add [origin] [仓库地址]

    添加一个远程连接

    git remote -v

## 1.5. git add

尽量多做

    git add .  
    
    把我们当前目录下面的所有文件，添加到***待提交***中,暂时还没生成版本

## 1.6. git commit -m ""

尽量多做

    git commit -m ""

    可以简单的理解为保存代码版本

    git log / git reflog

## 1.7. git reset [版本编号] [--hard]

    跳转到某个版本（状态、state）

## 1.8. git pull/git push

    git pull [远程连接名字] master:master
                           远程   本地      

    git push [远程连接名字] master:master
                           本地   远程 
                           
                           master 


    git pull origin master

# 2. HTML

## 2.1. 标签

一般而言，都是小写，除了DOCTYPE

一般而言，都是成对出现，某些例外,如：
```html
    <br/>
    <hr/>
    <img src="../background.jpg" alt="">
```

## 2.2. 嵌套

一般而言，标签都可以嵌套，但是部分标签不行

h1-6

p

## 2.3. 注释

```html
<!-- 注释 -->
```

## 2.4. 属性

必须在开始标签中，大多数html标签，都有共同的属性，但是也有各自特殊的属性

标准属性：id class title style

常见事件：onclick ondbclick onmoveover

style是标准属性中比较特殊的一种，跟css相关

事件是一种特殊的属性，跟js相关

HTML5 还支持自定义属性

## 2.5. head部分

meta charset keywords description

title

link

script

## 2.6. src href 寻址方式

/      返回顶级目录 
./     当前目录
../    上一级目录

## 2.7. 文本标签

b 粗体
i 斜体
u 下划线文本
del 删除线文本
sub 上标
sup 下标

h1-h6 1-6级标题
 
p 段落标签

br 换行标签

hr 分割线标签

# 3. 作业
使用以上文本标签，完成该页面的内容部分排版
[作业地址](http://www.unnuo.com/%E5%89%8D%E7%AB%AF%E5%9F%BA%E6%9C%AC%E7%9F%A5%E8%AF%86%E7%BB%93%E6%9E%84.html)