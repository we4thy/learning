# 攻击验证机制

## 验证技术

- 基于HTML表单的验证
- 多元机制，如阻隔密码和物理令牌
- 客户端SSL证书或智能卡
- HTTP基本和摘要验证
- 使用NTLM或HKerberos整合Windows的验证
- 验证服务

## 验证机制设计缺陷

### 密码保密性不强

- 密码短或空密码
- 常用的字典词汇或名称为密码
- 密码和用户名相同
- 仍然使用默认密码

### 蛮力攻击登录

### 详细的失败消息

### 证书传输易受攻击

可以进行攻击的攻击者位置：
- 用户的本地网络中
- 用户的IT部门内
- 用户的ISP内
- 因特网骨干网上
- 托管应用程序的ISP内
- 管理应用程序的IT部门内

不安全的原因：
- 以查询字符串参数而不是在POST请求主体中传送证书
- 以重定向的方式处理登录请求，以查询字符串参数的形式提交证书
- 应用程序将用户证书保存在cookie中

### 密码修改功能

通过此功能可以获取到的信息：
- 提供详细的错误信息，用户名是否有效
- 允许攻击者无限制猜测“现有密码”
- 允许攻击者不需入侵捷克成功查明现有密码

### 忘记密码功能

常见的功能设计缺点：
- 向用户提出一个次要质询以代替主要登录功能
- 存在无限制尝试回答密码质询安全漏洞
- 存在提供简单密码暗示
- 正确响应一个质询后，可以重新控制账户

### 记住密码功能

主要是对cookie的使用

### 用户伪装功能

功能上的设计缺陷：
- 一般通过隐藏功能的形式执行，不受常规访问控制管理
- 用户进行伪装时。应用程序可能会信任由用户控制的数据
- 存在提权漏洞

### 证书确认不完善

### 非唯一性用户名

存在的缺陷：
- 存在共同使用同一个密码错情况
- 攻击者实行统一用户名注册，对注册的返回进行观察

### 可预测的用户名

### 可预测的初始密码

### 证书分配不安全

## 验证机制执行缺陷

### 故障开放登录机制

### 多阶段登录机制中的缺陷

存在的缺陷：
- 系统会任务完成深层阶段验证的用户以完成低层次的验证，使得用户获取更多没有验证的权限
- 对不同阶段验证的值进行修改，修改验证标记，进行权限提升
- 每个验证阶段的用户身份不断变化，对用户的身份确定不明显

### 不安全的证书存储

## 保障验证机制的安全

主要考虑的因素：
- 应用程序所提供的功能和安全程度
- 用户对不同类型的验证控制的容忍和接收程度
- 支持一个不够友好的用户界面系统所需要的成本
- 竞争性解决方案相对于应用程序可能产生的收入方面的金融成本或它所保护的资产的价值

### 使用可靠的证书

- 强制密码复杂度
- 用户名唯一
- 用户名足够随机，不包含任何顺序

### 安全处理证书

- 对创建、保存和传送证书进行保障
- 密码定期修改
- 移出不安全的功能
- 使用尽可能安全的方式传送证书

### 正确确认证书

- 完整性
- 主动防御未知异常程序处理
-

### 防止信息泄露

### 防止蛮力攻击

### 防止滥用密码修改功能

### 防止滥用账户恢复功能

### 日志、监控与通知


