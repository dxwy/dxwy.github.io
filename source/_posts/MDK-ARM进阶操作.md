---
title: MDK-ARM进阶操作
date: 2021-01-03 20:44:09
categories: 软件使用笔记
tags: 
    - 笔记
    - 软件
---

## 一、添加插件

### 1、Astyle：一键格式化代码

Command：Astyle.exe路径
Arguments：$E*.c $E*.h

![image.png](Astyle.png)

### 2、FileComments：文件注释

Command：FileComments.exe路径
Arguments：!E

![image.png](FlieComments.png)

### 3、FunctionComment：函数注释

Command：FunctionComment.exe路径
Arguments：!E ~E

![image.png](FunctionComment.png)

### 4、DateTime：当前日期

Command：DateTime.exe路径
Arguments：!E ~E ^E

![image.png](DateTime.png)

### 5、DateTime：当前时间

Command：DateTime.exe路径
Arguments：!E ~E ^E T

![image.png](DateTime2.png)

## 二、KEIL工程文件说明

![image.png](KEIL工程文件说明.jpg)

## 三、使用git

### 1、加载SVCS

![image.png](加载SVCS.png)

### 2、修改Stage：一键添加所有修改

可以做如下修改一键添加所有代码

| Stage '%F' | -> | Stage all |
| :---: | :---: | :---: |
| add '%F' | -> | add -all |

![image.png](一键添加所有修改.png)

### 3、将日志文件添加.gitignore

工程编译后会生成很多编译文件，我们可以忽略这些文件的修改

```c
!*.c 
!*.h
*.log
*.plg
*.bak
*.dep
*.uvguix.*
JLinkLog.txt
*.o
*.d
*.crf
*.tra
*.axf
*.hex
*.lnp
*.sct
*.__i
*.htm
*.map
```

### 4、使用命令

![image.png](使用命令.png)

## 四、参考链接

[Keil的几个插件](https://blog.csdn.net/xinxinsky/article/details/79204763)
