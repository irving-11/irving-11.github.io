---
layout: post
title: C++调用.c文件的函数时出现undefined reference to...问题
categories: “坑”
description: 对学习过程中出现问题的一点汇总
keywords: C,C++,Problems
---

## 问题
  
在.cpp文件中调用.c文件中的函数时，即使在.cpp文件中include了c文件的头文件，然是在编译cpp文件时，仍然会报undefined reference to...错误，如图所示，

![alt 问题截图2](D:/myGithubSite/irving-11.github.io/images/posts/forPost/2.png)

![alt 问题截图1](D:/myGithubSite/irving-11.github.io/images/posts/forPost/1.png)




####网上给出的一般答案是这样的
![alt 问题截图3](D:/myGithubSite/irving-11.github.io/images/posts/forPost/3.png)  


但是对我来说“然并卵”，最后在一个论坛上找到了答案：
**需要把要引入的.c文件与.h文件都加入到.cpp文件所在工程中一起编译**  
即  
![alt 问题截图4](D:/myGithubSite/irving-11.github.io/images/posts/forPost/4.png)

