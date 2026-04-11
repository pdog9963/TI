### “随国家网络治理不断完善，简中网络能够轻易获取翻墙知识的时代业已逝去，而使翻墙一行为艺术传承的任务已让老师博们心力憔悴!~~(毕竟多数需亲自指导【doge】）~~

##### 此背景下，本项诞生了，意在帮助一些新手一站式学习翻墙工具、方法，及注意事项。下文从~~四~~两个”角色“所对应方法进行简述

  [![邮箱](https://img.shields.io/badge/Email-SZKG%40p11451.cloudns.be-brightgreen "邮箱")](https://img.shields.io/badge/Email-SZKG%40p11451.cloudns.be-brightgreen "邮箱")

****  
### *必要的科普*   
##### 希望我不需要科普GitHub的用法[包括如何从Releases下载内容]

<details>  
<summary>🧐点击展开</summary>  

#### 1. 什么是节点？   
节点 = 一个具体的代理服务器（可简称“服务器”或“Proxy”）。它包含：服务器IP地址、端口、协议类型（VMess、VLESS、Trojan、Shadowsocks等）、密码/UUID、加密方式等信息。   
作用：设备通过这个“节点”中转流量，实现科学上网（绕过GFW等设施）。  
一个好的节点通常有低延迟、高速度、解锁Netflix/YouTube等流媒体的能力。    

#### 2. 什么是订阅链接？  
订阅链接（Subscription URL）就是一个特殊的网页链接（通常以 https:// 开头），里面打包了很多节点的信息。将这个链接粘贴到Clash / v2rayN 等客户端里，客户端下载、解析、更新节点。    
优点：一键导入几十甚至几百个节点，不用手动一个一个添加。  
支持自动更新：节点失效了，点击“更新订阅”就能换新的。[在订阅链接失效]  
不同客户端有不同格式：Clash用YAML格式，v2rayN常用Base64或txt格式。  

类型：Clash专用订阅（.yaml格式）  
v2rayN / 小火箭通用订阅（v2ray / base64格式）  
付费机场的订阅链接通常带密钥（uuid/token）（很长一串），[免费的公开分享。形式通常与付费订阅相同，少数'无乱码'（即密钥）]  

#### 3. 什么是“订阅链接型的代理工具”？  
指Clash（Clash for Windows、Clash Verge、Clash Meta等）、v2rayN、NekoRay、sing-box 等这类开源/社区客户端。它们的共同特点是：支持订阅链接一键导入大量节点。  
高度可定制：可以自己写规则（比如国内直连、国外走代理、特定域名走特定节点等）。  
支持多种协议（VMess、VLESS、Trojan、Hysteria2、ss等），兼容性强。  
免费使用客户端本身，但节点通常来自“机场”（付费订阅服务），免费分享，[牢玩家去试试自建节点吧~]。  
适合高玩，它们功能强大、规则灵活、可以精细控制流量。  
### 项目推荐  
[NekoBox for Android](https://github.com/MatsuriDayo/NekoBoxForAndroid/releases "NekoBox for Android")，[v2rayN(电脑端的)](https://github.com/2dust/v2rayN/releases "v2rayN")， 
[Clash Verge(电脑端的)]([](https://github.com/clash-verge-rev/clash-verge-rev/releases) "Clash Verge")，
[v2rayNG](https://github.com/2dust/v2rayNG/releases "v2rayNG")，
[Clash Meta for Android](https://github.com/MetaCubeX/ClashMetaForAndroid/releases "Clash Meta for Android")   
  
  [nekobox使用教程](https://socks5ip.com.cn/dailigongju/nekoboxshiyongjiaocheng/ "nekobox使用教程")，v2rayNG,clash也类似

<details>  
<summary>🧐折叠的图片（安卓端代理工具示例</summary>  

<img src="https://github.com/pdog9963/TI/blob/main/photo/%E5%AE%89%E5%8D%93app.jpg?raw=true" width="210px">   

</details>  

这类工具本质上是代理客户端，而不是完整的VPN服务。  
 
 #### 4. “订阅链接型的代理工具”与快连VPN、黑石VPN 等“传统VPN”的区别  
“订阅链接型的代理工具”通常开源，不提供节点，但各方面都更为灵活，如分流代理，传输协议前沿（大佬们有很多持续的开源vpn协议项目），抗封锁强   
传统VPN则较于方便，通常为傻瓜式的，自定义弱，协议较少（通常闭源)   

##### 简单说：订阅链接 = 批量节点配置的“快递单”，客户端拿着这个单子去取货（节点）。
##### 值得注意的是 ~~（或许）~~ 提供订阅链接的服务器常与节点(代理)服务器分离。

</details>  

## **[START]**  

### **一、*"略爱折腾的穷小伙"***~~(简直本人)。~~ *[这些家伙不相信"天下没有免费的午餐",但忽视投入的时间]*   
**1.Vpn大法!** ~~快连~~，袋鼠，绿茶等vpn自然好用，但收费成为了其痛点。  
于是便有了XP/Lsp模块大法！实现会员订阅的破解，或“无限试用”。  
推荐项目：[Deer God](https://github.com/Xposed-Modules-Repo/com.wengui.hook "Deer God")，[Fuck for VIP](https://github.com/bug-bit/fckvip "Fuck for VIP")  
**·示例(Deer god)**  

<details>  

<summary>😄折叠示例</summary>  
<img src="https://github.com/pdog9963/TI/blob/main/photo/deer%20god%E7%A4%BA%E4%BE%8B.jpg?raw=true" width="210px"><img src="https://github.com/pdog9963/TI/blob/main/photo/%E9%97%AA%E8%BF%9Evpn%E7%A4%BA%E4%BE%8B.jpg?raw=tru" width="210px">  

以闪连vpn为例，注册后拥有三天会员，无需绑定。所以进行依靠模块清理本地数据，重新注册账号即可(注册用时小于30s)😋
  
</details>  




##### 但是，此方法弊端也十分明显：适用平台较窄。此处仅有关于root后安卓设备的介绍。

**2.自建节点** 没错！

## 穷小伙也能自建节点!🥰

**牢苟**最喜欢的项目[【youtube】 【2026最强】免费VPN节点！Cloudflare 10分钟搭建|永久免费|全球高速节点|4K8K秒开|无限流量](https://www.youtube.com/watch?v=okjTFMiUCYA "【youtube】 【2026最强】免费VPN节点！Cloudflare 10分钟搭建|永久免费|全球高速节点|4K8K秒开|无限流量")，***项目地址***[**edgetunnel**](https://github.com/cmliu/edgetunnel "🚀 edgetunnel")
推荐通过cloudflare pages搭建，配合代理工具（如v2ray）,秒杀大部分“机场”

**·值得注意的是，大部分claudflare节点搭建教程中都含“自定义域名”部分，然而这不是必须的，(cloudflare works与pages及其提供的域名会被"墙"，教程中多数免费域名同样会被"墙"，无法起代理作用），可以在连接代理环境下更新订阅组**  

<details>  
  
<summary>🧐折叠的图片（节点示例</summary>  

<img src="https://github.com/pdog9963/TI/blob/main/photo/v2rayn.png?raw=true" width="400px">  

<img src="https://github.com/pdog9963/TI/blob/main/photo/%E8%8A%82%E7%82%B9%E5%AE%9E%E4%BE%8B.png?raw=true" width="400px">  


</details>

****

### **二，*"不爱折腾的穷小伙"*** *[糟糕透了，他们什么都不愿付出]*

###### 极低的投入带来了较差的体验（对于本段大部分来说），高ping，底带宽，以及消失的安全性。

**1，免费VPN工具** ；不作推荐、仅举例。如[**hiddify**](https://hiddify.com/ "hiddify")等。存在以上问题。  
### **2，免费节点!**   
从公开信息中寻找订阅链接，缺点在于节点多人使用，低带宽，额度（流量）“光速”归零，需不断寻找新的订阅。  

①.Teleglam. 电报（纸飞机）上存在大量订阅分享频道，如[**轩辕节点吧**](https://t.me/fq521)；可使用点*搜索bot*（如：[**极搜**](https://t.me/jisou "极搜"))  

<details>  
<summary>😋折叠的图片（极搜</summary>  
  
<img src="https://github.com/pdog9963/TI/blob/main/photo/ScreenShot_2026-04-11_134149_802.png?raw=true" width="400px">  

</details>

②Grok：[万能的Grok啊] *“  **Grok!**  我要一些适用于clash,v2rayn的订阅链接”*   

<img src="https://github.com/pdog9963/TI/blob/main/photo/grok%E7%A4%BA%E4%BE%8B.png?raw=true" width="400px">   

③GitHub  不用多说，GitHub内直接搜索 ,**[显而易见的是，Grok提供的许多免费订阅链接都源于Github！]**   
  <img src="https://github.com/pdog9963/TI/blob/main/photo/GitHub%E6%90%9C%E7%B4%A2%E7%A4%BA%E4%BE%8B.png?raw=true" width="400px">  
  
*相信够用，不多介绍*  
**3.乞讨去吧！**  ~~（本段内最优解）~~  
①在公开媒体乞讨如X（最好别在国内平台上）   
②.联系好友发出请求  
<img src="https://github.com/pdog9963/TI/blob/main/photo/%E4%B9%9E%E8%AE%A8%E7%A4%BA%E4%BE%8B.jpg?raw=true" width="210px">  

### 其实还剩两个角色[分别是'爱折腾的富哥'与'不爱折腾的富哥']，奈何精力不足，缺乏经验，难以写完。甚是遗憾！
##### 可以试试联系牢苟哟~，小概率会获得订阅链接~~
