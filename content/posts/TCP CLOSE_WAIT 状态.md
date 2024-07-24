---  
share: true  
title: TCP CLOSE_WAIT 状态  
date: 2024-07-18  
tags:  
  - 笔记  
  - 计算机_网络  
  - 完成  
---  
  
#笔记 #计算机/网络 #完成   
  
![markdown/20240718150619.png|800](http://note.img.lixd.club/markdown/20240718150619.png)  
  
TCP CLIENT 与 SERVICE 的状态转移表。  
  
CLOSE_WAIT 的状态形成是： 客户端主动关闭 发送 `FIN` + `ACK` 标志包给 SERVICE。此时的 服务器状态变为 ==CLOSE_WAIT==。  
若 服务器没有对 被动关闭做相关处理，或相关逻辑已经发生异常。则 CLOSE_WAIT 状态将会保持于该进程重启前。