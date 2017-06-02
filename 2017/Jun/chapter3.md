# Web应用程序技术

## HTTP

### HTTP请求

- 一个说明HTTP方法的动词，一般有GET POST等
- 所请求的URL
- 使用的HTTP版本
- Referer，消息头，用于发出请求的原始URL
- User-Agent，客户端相关信息
- Host，完整URL的主机名
- Cookie，用于提交服务器向客户端发布的其他参数

### HTTP响应

- 使用的HTTP版本
- 请求结果状态码
- 原因短语，进一步说明相应状态
- Server，指明所使用的Web服务器软件
- Set-Cookie，用于向浏览器发送另一个cookie
- Pragma，指定浏览器不要将响应保存在缓存中
- Content-Type，用于表示消息主体的类型
- Content-Length，消息主体的字节长度

### HTTP方法

常用的方法

- GET，用于获取资源
- POST，用于执行操作
- HEAD，方法与GET方法相似，不同之处在于服务器不会在其影响中返回主体
- TRACE，用于诊断，检测客户端与服务器之间是否存在代理
- OPTIONS，要求服务器报告对于某一特殊资源有效的HTTP方法
- PUT，使用包含在请求主体中的内容，向服务器上传指定的资源

### URL

统一的资源定位符

### REST

表述性状态转移，分布式系统的一种体系架构

### HTTP消息头

1. 常用的消息头

- Connection，告诉HTTP传输后的TCP连接关闭情况
- Content-Encoding，消息主体中的内容指定编码形式
- Content-Lenth, 规定消息主体的字节长度
- Content-Type，规定消息主体的内容类型
- Transfer-Encoding，指定为方便其通过HTTP传输而对消息主体使用的任何编码

2. 请求消息头

- Accept，用于告诉服务器客户端愿意接受哪些内容
- Accept-Encoding，用于告诉服务器接受哪些内容编码
- Authorization，用于为一种内置HTTP身份验证向服务器提交证书
- Cookie，用于向服务器提交它以前发布的cookie

3. 响应消息头

### cookie

### 状态码

- 1XX —— 提供信息
- 2xx —— 请求被成功提交
- 3xx —— 客户端被重定向到其他资源
- 4xx —— 请求包含某种错误
- 5xx —— 服务器执行请求时遇到错误

### HTTPS

### HTTP代理

### HTTP身份验证

- Basic
- NTLM
- Digest

## Web功能

### 服务器端功能



