---  
share: true  
title: LINUX 最大句柄限制  
date: 2024-07-08  
tags:  
  - 笔记  
  - 计算机_操作系统  
  - 完成  
---  
  
  
#笔记 #计算机/操作系统  #完成  
  
LINUX 的文件概念范围比较大，真实的文件以及 SOCKET 均可以被归纳在文件内。LINUX 对打开的文件句柄数量有限制。即 LINUX 系统对运行的==进程==从系统资源中申请句柄数存在默认限制。  
  
目前查看 DOCKER 对句柄数的相关解释已知，DOCKER 程序对其进程最大打开句柄数没有做限制。   
  
[DOCKER 最大打开句柄数没有限制](https://github.com/containerd/containerd/pull/7566)  
  
