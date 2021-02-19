---
title: TCP连接过程
date: 2021-02-19 22:02:16
tags:
---

# 三次握手
* client -> server SYN=1 seq=x
* server -> client SYN=1 ACK=1 seq=y ack=x+1
* client -> server ACK=1 seq=x+1 ack=y+1
# 四次挥手
* client -> server FIN=1 seq=u
* server -> client ACK=1 seq=v ack=u+1
* server -> client FIN=1 ACK=1 seq=w ack=u+1
* client -> server ACK=1 seq=u+1 ack=w+1

# 四次挥手的原因
服务器收到消息可能还有数据需要发送,所以只能先回复ACK,然后才回复FIN

# 四次挥手client最后等待的原因
防止服务器没收到最后一次信息而未正确断开连接

# 三次握手的原因
保证client和server有相互之间发送数据的序列号