---
layout: post
lang: zh-CN
title: "2026 TiviMate 配置 TVB 翡翠台完整教程"
date: 2026-10-15 09:00:00 +0800
comments_id: zh-tvb-jade-tivimate-2026
description: "港人移民想看 TVB 港剧综艺的诚实对比与配置指南。"
target: 港人移民想看 TVB 港剧综艺
---

# TiviMate 配置 TVB 翡翠台直播：M3U 导入完整教程

> 目标读者：在海外（英国、澳大利亚、加拿大、美国）生活的港人 / 粤语用户，想在 TiviMate 上直接看 TVB 翡翠台 24 小时直播流。本文是一份**纯技术教程**，不评论任何频道内容来源的版权状态。


## 二、找 M3U 订阅之前，先认识三种"TVB 频道"

在搜索 M3U 列表时，不同服务商对 TVB 频道的命名差异很大，**先确认你要找的是哪个**：

| 频道名 | 实际内容 | 24h 直播？ |
|--------|----------|-----------|
| TVB 翡翠台（TVB Jade） | TVB 主频道，新闻 + 港剧 + 综艺 | 是 |
| TVB 明珠台（TVB Pearl） | TVB 英语 / 普通话二台 | 是 |
| TVB Plus / TVB J2 | 年轻向 / 综艺 / 信息台 | 是 |
| myTV SUPER 独家频道 | myTV SUPER App 内专属流 | 不是 24h 卫星直播 |

**只有"TVB 翡翠台"才是老港人习惯看的那个**。列表里写"TVB 港剧点播"或"TVB Plus"是另一个东西。

---

## 三、现有方案对比

下面是截至 2026 年 10 月，海外港人看 TVB 翡翠台的五种路径。**所有价格来自各服务公开标价**。

| 方案 | 月费 | 是否 TVB 翡翠台 24h 直播 | 设备 | 维护 |
|------|------|--------------------------|------|------|
| **TVB Anywhere+ 官方 App** | **$17 加币/月** 或 $180/年 | 有（北美版）/ 受限（其他地区）| 智能电视 / 手机 / Apple TV / Fire TV | 低 |
| KyLinTV | $19.99-25.99 加币/月 | 有 | 智能电视 / 机顶盒 | 低 |
| 公开 GitHub M3U 列表 | $0 | 部分有（标 "TVB" / "Jade"）| 任意 M3U 播放器 | 极高（频道易失效）|
| 付费 M3U 订阅 | $5-10/月 | 通常有（**下单前需确认**）| TiviMate / Televizo | 中 |
| myTV SUPER App（香港版） | 38 HKD/月 | 有完整版权 | 需要 VPN + 香港 IP / 香港手机号注册 | 高（账号易失效）|

几点**事实陈述**，不评价优劣：

1. **TVB Anywhere+ 北美版**官方注册页 17 加币/月或 180 加币/年。**注意**：**只覆盖 TVB 自家频道和精选港剧**——不是 TVB 所有版权内容。比如香港赛马、TVB 节目回看超过 7 天的内容都不在 Anywhere+ 套餐内。
2. **myTV SUPER 是香港本地版**，**38 HKD/月，海外 IP 访问会被拒绝**。海外港人看 myTV SUPER 必须用 VPN + 香港手机号 + 香港银行或 FPS 支付，**这条路径劝退率 90% 以上**。
3. **M3U（*.m3u / *.m3u8）是一种公开的播放列表文件格式**，任何人都可以生成、分享、修改。**该格式本身只是技术规范，不绑定任何具体频道或内容来源**。M3U 订阅服务的合法性，取决于其内容来源是否获得授权。
4. **KyLinTV 的"Cantonese Pack"在基础包内**——但**不是所有基础包都包含**。下单前向客服明确问"包含哪些粤语台"。

---

## 四、技术路径：TiviMate + 订阅链接

### 硬件（一次性）

- **Amazon Fire TV Stick 4K Max**：美国 Amazon $89.48，加拿大约 $119 CAD（2026 年 10 月查询）。TiviMate 在 Fire TV 上运行最稳定。
- **NVIDIA Shield TV Pro**：美国 $199，加拿大约 $279 CAD。性能更强，但多数场景 Fire TV Stick 4K Max 足够。
- **任何 Android TV 智能电视**（Sony、TCL、海信）：内置 Google Play，可直接装 TiviMate。

不建议买的：

- 标称"亚洲电视""港台电视"的**预付费机顶盒**（UBOX、EVPad、SviCloud 等）：硬件本身是廉价 Android 盒子，**核心依赖里面的 M3U 订阅服务**。服务方随时可以停售，盒子变砖，无售后。
- 任何要求"必须搭配我们的盒子才能用"的 M3U 订阅：好的订阅应该是一段 URL，**你换任何设备都能用**。

### 软件：M3U 播放器

**M3U 播放器只负责读取播放列表、显示节目指南（EPG）、发送播放请求**。它本身不提供任何内容，所有内容来自你导入的 M3U 链接。

| 平台 | 推荐播放器 | 备注 |
|------|-----------|------|
| Android TV / Fire TV / Shield | **TiviMate** | 界面最接近传统有线电视的节目指南；官网 tivimate.com 明确说明"TiviMate is a media player only and does not provide any content" |
| Android TV / Fire TV / Shield | **Televizo** | Google Play 评分 4.0 / 17.7K 评价（com.ottplay.ottplay）；现代 UI，多播放列表；免费版可用，PRO 订阅解锁 5 设备 / 去广告 |
| iOS / iPadOS / Apple TV | **Smarters IPTV Player** | App Store 上架，开发者 Smarters；同样只读 M3U 链接，不提供内容 |
| iOS / iPadOS / Apple TV | **APTV** | App Store 上架（id 1630403500），开发者 Kimen；支持 iPhone / iPad / Mac / Apple TV / Apple Watch / Vision Pro 六个 Apple 平台 + CarPlay 视频投屏 |
| 任何平台 | **VLC media player** | 免费开源，支持 M3U；但不渲染 EPG 节目指南，需要自己整理频道 |

### TiviMate 配置步骤

TiviMate 在 Google Play 上免费版可以导入 M3U，**完整功能（EPG 渲染、录制、多设备同步）需要 In-App Purchase 订阅**。**官方未公开具体订阅价格**（截至 2026 年 10 月查询），下单前以应用内显示为准。

1. **安装 TiviMate**：在 Fire TV 上打开 Google Play，搜 "TiviMate"，开发者为 AR Mobile Development。或者从 tivimate.com/apk 下载 sideload 安装包。
2. **准备 M3U 订阅链接**：通常是你付费订阅后，服务商通过邮件或后台给你的一个 URL，形如 `https://example.com/sub/your-code.m3u`。**只订阅明确列出 TVB 翡翠台的套餐**，下单前在服务商的频道列表里搜"TVB Jade"或"翡翠"确认。
3. **配置 M3U 链接**：打开 TiviMate → Settings → My Playlists → Add playlist from URL，粘贴订阅链接 → 保存。
4. **等待列表加载**（通常 10-30 秒），频道数量可能几百到几千不等。
5. **搜索 TVB 频道**：在频道列表顶部搜索框输入 "TVB"，把 **TVB 翡翠台（Jade）**、**TVB 明珠台（Pearl）**、**TVB Plus / J2** 等加进收藏。
6. **配置 EPG**（可选但推荐）：TiviMate → Settings → EPG → Add EPG source，通常 M3U 订阅商会同时提供 XMLTV 格式的 EPG 链接，填进去。**有 EPG 之后界面就是传统有线电视的样子**——按时间表看今晚 8 点。
7. **测试稳定性**：香港黄金时段（北京时间晚 8-10 点 = 美东时间早 7-9 点 / 美西时间凌晨 4-6 点）流量最大，是真实场景测试。

**iOS / iPadOS / Apple TV 用户**用 Smarters IPTV Player 或 APTV，配置流程一样（Smarters：底部 Login → Add User via M3U URL；APTV：底部 Sources → Add Source → M3U URL）。

### 父母使用

配好之后，给父母一个简化的遥控器说明：

- **左右键**：切换频道（你帮他们把 TVB 翡翠台、TVB 明珠台、TVB Plus 放在收藏前 3 位）。
- **上下键**：换频道。
- **OK 键**：进入节目单（EPG）。
- **返回键**：回到主界面。

**不要让父母接触 M3U 链接或订阅续费**。TiviMate 有"家长控制 / PIN 码"功能，开启后他们无法误删播放列表；Televizo 同样支持 PIN 锁定。

---

## 五、常见问题

**Q1：TiviMate 多少钱？**

A：TiviMate 免费下载，订阅价格在 Google Play 应用内显示。**官方不公开统一价目**，不同地区、不同时期可能不同。下单前以应用内显示为准。

**Q2：M3U 列表里有"TVB"但播放黑屏怎么办？**

A：三种常见原因：
1. **M3U 列表里的链接已失效**（上游 CDN 换了地址）—— 跟服务商要最新链接。
2. **频道需要地域限制**（如 TVB 部分流只允许香港 IP 播放）—— 尝试在 TiviMate 里给该频道绑代理。
3. **你的 M3U 订阅商根本拿不到 TVB 翡翠台的 24h 直播流**——只有标"翡翠台点播"或"港剧回看"，**没有真正 24h 卫星直播**。这种情况换服务商。

**Q3：TVB Anywhere+ 能在 TiviMate 里看吗？**

A：不能。TVB Anywhere+ 是封闭 App，不开放 M3U 链接。**它走自己的 DRM 加密流**，TiviMate 读不到。要么在 TVB 官方 App 里看，要么用 M3U 订阅走另一条路径——**两个不能合并**。

**Q4：EPG 节目指南数据从哪来？**

A：EPG 是另一条数据流，**和 M3U 分开**。常见来源：
1. **M3U 订阅商自带**（通常 M3U 链接下面会附一个 XMLTV 链接，填到 TiviMate EPG 设置里）
2. **公开 EPG 源**（如 epg.iptvx.top 等社区维护的源）——质量参差，**且部分源要求付费**。
3. **自己用 xmltv-grabber 抓取**——技术门槛高，不推荐非技术用户。

**Q5：TiviMate 的录制功能能用吗？**

A：TiviMate Premium 的"录制"是**客户端级**——把直播流实时缓存到 Fire TV Stick 的本地存储（32GB 模型可用空间约 14GB，**约能录 6-8 小时标清 / 3-4 小时高清**）。**不是 DVR 服务器级录制**——不能远程预约、不能异地看。

---

## 六、结论

对于"在 TiviMate 上看 TVB 翡翠台 24h 直播"这个需求，**2026 年最稳的方案是**：

- **硬件**：Amazon Fire TV Stick 4K Max（$89.48 USD，一次性投入）
- **播放器**：TiviMate（Android 平台）；iOS 用户用 APTV 或 Smarters IPTV Player
- **订阅**：月费 $5-10 USD 的 M3U 订阅，**下单前确认频道列表里有 TVB 翡翠台（标"TVB Jade"）**
- **EPG**：向订阅商要 XMLTV 链接填进 TiviMate → Settings → EPG
- **VPN**：不需要（M3U 路径）；TVB 官方 App 不需要

**完全合规、不碰 M3U**的家庭直接用 TVB Anywhere+ 官方 App，**但要接受北美版内容比香港版少**这一事实。

---

## 七、商业化服务

如果你希望跳过 GitHub 列表的频繁失效、跳过手动配置 M3U 链接的过程，可以查看本项目 GitHub 主页（`README` 里的 **"商业化服务"** 板块）了解作者提供的付费订阅配置：包含维护好的 TVB 翡翠台 / 明珠台 / J2 频道列表、自动续费的订阅链接、以及 7 天试用入口。

> 本文所有价格与功能描述均来自各服务在 2026 年 10 月的公开页面，可能随时变动。下单前请以官网当时显示为准。

---

## 直接试用作者的方案

如果你想跳过上面说的手动 M3U 配置流程，作者维护一个付费订阅服务：维护好的中文频道列表、自动续订链接、7 天试用入口。

**免费试用 7 天** — 试用期间不需付款。试用结束后服务 **$9.99/月**（最少 3 个月）或 **$59.88/年**（省 50%）。

<p><a class="cta-button" href="https://iptv-search.com/login?tab=register&utm_source=github-pages&utm_medium=seo-article&utm_campaign=zh-tvb-jade-tivimate-2026" target="_blank" rel="noopener">免费试用 7 天 →</a></p>

注册后会自动获得订阅链接和 7 天 VIP 试用。

> 本文所有价格和功能描述均来自各服务公开页面（2026 年 10 月），随时可能变动。请在购买时以官网为准。