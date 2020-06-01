---
layout: post
title:  "C++调用.c出现underfined reference to...问题"
date:   2020-03-23 21:03:36 +0530
categories: C++ 
---

在.cpp文件中调用.c文件中的函数时，即使在.cpp文件中include了c文件的头文件，然是在编译cpp文件时，仍然会报undefined reference to...错误，如图所示，

<img src="../assets/images/2.png" alt="图2" />

<img src="../assets/images/1.png" alt="图1" style="zoom:67%;" />

网上给出的一般答案是这样的

<img src="../assets/images/3.png" alt="图3" style="zoom:80%;" /> 

但是对我来说“然并卵”，最后在一个论坛上找到了答案：
**需要把要引入的.c文件与.h文件都加入到.cpp文件所在工程中一起编译**  
即  

<img src="../assets/images/4.png" alt="图4" style="zoom:80%;" />

