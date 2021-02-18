---
title: Http返回值
date: 2021-02-18 22:03:26
tags:
---

# 1xx
信息提示
* 101 Switching Protocols 转换协议(websocket中会用到)

# 2xx
成功
* 200 OK 正常

# 3xx
重定向
* 304 NotModified 见[缓存](2021/02/01/浏览器缓存策略/)

# 4xx
客户端错误
* 400 BadRequest 请求错误
* 404 Not Found 未找到

# 5xx
服务器错误
* 500 InternalServerError 服务器内部错误