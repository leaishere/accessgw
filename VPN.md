

# 自研VPN加密方案

##### 原因：

-  IPSEC等VPN协议，有时会被定向封锁或误杀

- GRE、OpenVPN、IPSEC等主流协议均
   较容易针对

- 一般封锁针对：（UDP/TCP，端口号） 或者IP报文中的协议编号字段

  

##### 解决思路：

- 使用更加”静默“的协议。

- 定制化混淆，并长期维护。

- 使用wireguard协议。wireguard设计思路：
 没有认证的报文不响应，不会被网络扫描、探测到不同于IPSEC、TLS，无加密协商过程
  混淆wireguard协议。VPN协议受关注，容易被误杀。
  自研wireguard混淆方案，免费提供持续维护

