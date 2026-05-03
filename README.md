# 🚀 新手翻墙一站式指南

> 想科学上网但不知从何下手？这份指南帮你零基础入门，找到最适合你的方法。

---

## 📖 这个项目是什么？

简单说：**帮新手用最低成本（甚至零成本）学会科学上网**。

无论你是愿意折腾的"技术探险家"，还是只想点两下就能用的"佛系用户"，这里都有适合你的方案。

---

## 🔥 背景：为什么需要这份指南？

随着网络环境的变化，过去随手可得的翻墙教程越来越难找到。而那些掌握方法的老玩家们，也很难一一手把手教新人。

本指南的目标就是——**让你看完就能自己搞定**，不用求人 (๑•̀ㅂ•́)و✧

---

## ⚡ 快速开始（30 秒了解）

| 你的情况 | 推荐方案 | 预计耗时 |
|---------|---------|---------|
| 愿意动手学习 | [Cloudflare 自建节点](#-方案一cloudflare-自建节点推荐) | 10 分钟 |
| 完全不想折腾 | [找免费订阅链接](#-方法二寻找免费订阅链接) | 2 分钟 |
| 安卓已 ROOT | [破解 VPN 会员](#-补充破解-vpn-会员仅限安卓-root) | 5 分钟 |
| 有朋友在用 | [直接要一个节点](#-方法三直接向朋友求助) | 30 秒 |

---

## 📚 基础概念科普

> 第一次接触这些名词？别怕，看完下面四个概念你就入门了！展开查看详情 👇

<details>
<summary>🧐 点击展开：基础概念</summary>

### 1. 什么是「节点」？

**节点**就是一个代理服务器，它帮你把网络请求转发到国外，从而绕过防火墙。

一个节点通常包含：
- 服务器地址（IP）
- 端口号
- 协议类型（VMess / VLESS / Trojan / Shadowsocks 等）
- 密码或密钥
- 加密方式

> 💡 **简单理解**：节点就像一扇通往"外面世界"的门，你需要知道门的位置（IP）、用什么钥匙（密码）才能打开它。

一个好的节点通常具备：低延迟、高速度、能解锁流媒体（Netflix / YouTube 等）。

---

### 2. 什么是「订阅链接」？

**订阅链接**是一个特殊的网址，里面打包了多个节点的信息。

- 把链接粘贴到客户端 → 自动导入几十个节点 → 不用手动一个个添加
- 节点失效后点击「更新订阅」就能换新节点 → 省心
- 链接失效则无法更新 → 需要重新获取

**不同客户端用的格式不同**：

| 客户端 | 常用格式 |
|--------|---------|
| Clash 系列 | YAML（.yaml） |
| v2rayN / 小火箭 | Base64 或 txt |

订阅链接通常长这样（有些含混淆加密）：

<img src="https://github.com/pdog9963/TI/blob/main/photo/%E8%AE%A2%E9%98%85%E9%93%BE%E6%8E%A5%EF%BC%88%E6%9C%AA%E6%B7%B7%E6%B7%86%EF%BC%89.png?raw=true" width="400px">

*▲ 未混淆的配置*

<img src="https://github.com/pdog9963/TI/blob/main/photo/%E8%AE%A2%E9%98%85%E9%93%BE%E6%8E%A5%EF%BC%88%E6%B7%B7%E6%B7%86%EF%BC%89.png?raw=true" width="400px">

*▲ 混淆后的配置*

---

### 3. 「代理客户端」是什么？

代理客户端是安装在你的设备上的**软件**，用来连接节点、管理流量。

常见的开源客户端：

| 平台 | 推荐客户端 |
|------|-----------|
| 💻 Windows | [v2rayN](https://github.com/2dust/v2rayN/releases)、[Clash Verge](https://github.com/clash-verge-rev/clash-verge-rev/releases) |
| 📱 Android | [NekoBox](https://github.com/MatsuriDayo/NekoBoxForAndroid/releases)、[v2rayNG](https://github.com/2dust/v2rayNG/releases)、[Clash Meta](https://github.com/MetaCubeX/ClashMetaForAndroid/releases) |

> 📖 教程参考：[NekoBox 使用教程](https://socks5ip.com.cn/dailigongju/nekoboxshiyongjiaocheng/)（v2rayNG、Clash 操作类似）

<details>
<summary>📱 安卓端代理工具截图</summary>

<img src="https://github.com/pdog9963/TI/blob/main/photo/%E5%AE%89%E5%8D%93app.jpg?raw=true" width="210px">

</details>

---

### 4. 代理客户端 vs 传统 VPN

| 对比维度 | 代理客户端（Clash/v2rayN） | 传统 VPN（快连/黑石等） |
|---------|--------------------------|------------------------|
| 开源 | ✅ 通常开源 | ❌ 通常闭源 |
| 节点来源 | 自己找 / 订阅链接导入 | 官方提供 |
| 自定义规则 | ✅ 支持分流、规则定制 | ❌ 傻瓜式，不可定制 |
| 协议丰富度 | ✅ 支持多种前沿协议 | ❌ 协议较少 |
| 抗封锁能力 | ✅ 较强 | ⚠️ 一般 |
| 上手难度 | ⚠️ 需一定学习 | ✅ 开箱即用 |
| 是否免费 | 客户端免费，节点另算 | 通常收费 |

> 💡 **简单总结**：代理客户端功能更强、更灵活，但需要自己准备节点；传统 VPN 方便省心，但要花钱且自由度低。

</details>

---

## 🛠️ 方案一：Cloudflare 自建节点（⭐推荐）

> 适合愿意花 10 分钟动手的你。**免费、高速、无限流量**，效果秒杀大部分付费机场。

### 🎬 视频教程

[【YouTube】2026 最强免费 VPN 节点！Cloudflare 10 分钟搭建 | 永久免费 | 全球高速 | 4K 秒开 | 无限流量](https://www.youtube.com/watch?v=okjTFMiUCYA)

### 📦 项目地址

👉 [**edgetunnel**](https://github.com/cmliu/edgetunnel)

### 🛠️ 搭建方式

推荐通过 **Cloudflare Pages** 部署，配合 v2rayN 等客户端使用。

### ⚠️ 重要提示

- **自定义域名不是必须的**，很多教程让你绑域名只是锦上添花
- Cloudflare Workers 自带域名（`*.workers.dev`）可能被墙，**建议在已连接代理的环境下更新订阅**
- 很多教程里的免费域名同样会被墙，注意甄别

### 📸 效果展示

<details>
<summary>🧐 点击查看节点效果截图</summary>

<img src="https://github.com/pdog9963/TI/blob/main/photo/v2rayn.png?raw=true" width="400px">

<img src="https://github.com/pdog9963/TI/blob/main/photo/%E8%8A%82%E7%82%B9%E5%AE%9E%E4%BE%8B.png?raw=true" width="400px">

</details>

---

### 📎 补充：破解 VPN 会员（仅限安卓 ROOT）

> ⚠️ 该方法**仅适用于已 ROOT 的安卓设备**，且为临时方案，不保证长期有效。

利用 Xposed/LSPosed 模块实现会员功能破解或无限试用。

**推荐项目**：
- [Deer God](https://github.com/Xposed-Modules-Repo/com.wengui.hook)
- [Fuck for VIP](https://github.com/bug-bit/fckvip)

**操作示例**（以闪连 VPN 为例）：

<details>
<summary>😄 点击展开示例</summary>

<img src="https://github.com/pdog9963/TI/blob/main/photo/deer%20god%E7%A4%BA%E4%BE%8B.jpg?raw=true" width="210px">
<img src="https://github.com/pdog9963/TI/blob/main/photo/%E9%97%AA%E8%BF%9Evpn%E7%A4%BA%E4%BE%8B.jpg?raw=true" width="210px">

> 注册后获得 3 天会员（无需绑定），使用模块清理本地数据后重新注册即可循环使用（每次注册约 30 秒）。

</details>

---

## 🎁 方案二：免费资源（不想折腾版）

> ⚠️ 免费资源的代价：高延迟、低带宽、多人共用、流量很快耗尽、安全性无保障。适合临时使用或轻度需求。

### 方法一：免费 VPN 工具

不作具体推荐，仅举例说明（如 [Hiddify](https://hiddify.com/) 等）。这类工具普遍存在上述问题，体验一般。

---

### 方法二：寻找免费订阅链接

#### 🔹 Telegram（电报）

大量免费节点分享频道，推荐使用搜索 Bot：

- 📢 频道示例：[轩辕节点吧](https://t.me/fq521)
- 🤖 搜索 Bot：[极搜](https://t.me/jisou)

<details>
<summary>😋 点击查看极搜截图</summary>

<img src="https://github.com/pdog9963/TI/blob/main/photo/ScreenShot_2026-04-11_134149_802.png?raw=true" width="400px">

</details>

#### 🔹 Grok AI

直接向 Grok 提问：

> *"Grok！我需要一些适用于 Clash、v2rayN 的订阅链接"*

<img src="https://github.com/pdog9963/TI/blob/main/photo/grok%E7%A4%BA%E4%BE%8B.png?raw=true" width="400px">

> 💡 Grok 提供的免费链接**大多源自 GitHub**，所以不如直接去 GitHub 搜索～

#### 🔹 GitHub 搜索

直接在 GitHub 搜索相关关键词：

<img src="https://github.com/pdog9963/TI/blob/main/photo/GitHub%E6%90%9C%E7%B4%A2%E7%A4%BA%E4%BE%8B.png?raw=true" width="400px">

---

### 方法三：直接向朋友求助

有时候最简单的方案反而是最好的 😉

- 在 X（Twitter）等平台友善地请求
- 直接联系已经在用的朋友

<img src="https://github.com/pdog9963/TI/blob/main/photo/%E4%B9%9E%E8%AE%A8%E7%A4%BA%E4%BE%8B.jpg?raw=true" width="210px">

---

## ⚠️ 注意事项

- 🔒 **免费节点的安全性无法保证**，不要在使用免费节点时登录重要账号
- 🌐 Cloudflare Workers 自带域名在国内可能被墙，建议在代理环境下操作
- 🔄 订阅链接会定期失效，需要重新寻找
- 📱 破解 VPN 方法仅限安卓 ROOT 环境，普通用户请使用方案一或方案二
- ⏳ 免费节点的流量和带宽有限，多人共用时体验会明显下降

---

## 📎 参考资源与推荐阅读

- 📘 [防火长城笔记仓库](https://github.com/AntonyCheng/gfw-notes) —— 深入了解 GFW 原理
- 📄 [越过长城，走向世界——翻墙协议的历史与原理浅析](https://blog.ch3nyang.top/post/%E7%BF%BB%E5%A2%99%E5%8D%8F%E8%AE%AE/)
- 🛠️ [GitHub 使用基础](https://docs.github.com/) —— 如果你还不熟悉 GitHub 的操作

---

## 💬 联系作者

📧 邮箱：SZKG@p114514.cloudns.be

> 精力有限，指南难免有未覆盖之处。欢迎联系交流，但**不保证回复**哦～

---

*Last updated: 2026*

