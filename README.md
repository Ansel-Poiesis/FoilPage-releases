# 视频的二向箔 · FoilPage

在本机下载与转写视频，将内容整理为可阅读、可编辑的文稿。支持抖音、B 站、YouTube 与本地媒体。

源码在私有仓库维护，本仓库仅提供 Windows 安装包与更新说明。官方发行入口：[Ansel-Poiesis/shengjian-releases](https://github.com/Ansel-Poiesis/shengjian-releases)。

产品中文名为「视频的二向箔」，英文名为 FoilPage（1.3.4 曾用名 Clip to Page，因搜索辨识度不足更名）。**最新正式版为 [1.3.2](https://github.com/Ansel-Poiesis/shengjian-releases/releases/tag/v1.3.2-formal)（2026-10-31）——本地功能登录即用，取消解锁付费**；测试版为 [1.3.5](https://github.com/Ansel-Poiesis/shengjian-releases/releases/tag/v1.3.5)。

## 安装与首次使用

1. 从 [最新正式版](https://github.com/Ansel-Poiesis/shengjian-releases/releases/latest) 下载 `FoilPage-Setup-1.3.2.exe` 并安装。支持 Windows 10 1809 及以上、Windows 11 的 64 位系统，无需安装 Python 或 Node.js。
2. 打开二向箔，在「准备」依次完成邮箱登录、环境检测与保存目录设置、本地模型下载。
3. 完成准备后进入「任务」。可粘贴视频链接，也可在「导入媒体」拖入本地视频。

安装包包含 CPU 转写所需的运行组件。NVIDIA GPU 加速包为独立可选下载：选择与桌面版本匹配的 GPU 加速包；1.3.4 测试版文件为 `FoilPage-GPU-Pack-1.3.4.zip`，在「准备 → 环境检测 → 安装 GPU 加速包」中选取，完成后重启。CPU 用户无需下载该包。

## 试用、解锁与云端积分

账户首次启用可免费试用 **15 天**。到期后 **¥9.90 一次性永久解锁本地软件**，无需续费软件使用权；已购买的解锁状态在账户中显示。

| 方式 | 金额与额度 | 转写并发 |
| --- | --- | --- |
| 试用／无有效云端套餐 | 试用期或永久解锁后使用本地模型，不消耗二向箔积分 | 1 |
| 标准云端积分 | ¥19.80／500 积分／30 天 | 2 |
| 专业云端积分 | ¥49.80／2000 积分／30 天 | 4 |

云端积分按需单独购买，不自动续费。正文整理与标题优化分别启用、分别计量；自带密钥由对应模型服务商计费。软件解锁与云端充值分别下单，不会互相替代。付款、积分和有效期以应用内确认的订单与账户权益为准，更多说明见「订阅」里的帮助。

试用按邮箱计时，允许更换邮箱再次试用；同一邮箱重新登录不重置试用。切换账户保留本机视频与文本，充值权益属于对应账户。

正式版仅提供月付积分。测试版的年付入口仅作占位，暂不能购买；历史已成立订单保持原有权益。

## 浏览器扩展

首次打开二向箔的「浏览器」页，点击「打开扩展目录」。在 Chrome／Edge 的扩展管理页启用开发者模式，选择「加载已解压的扩展」，加载该固定目录。

默认目录为 `%LOCALAPPDATA%\Programs\VideoToArticle\browser-extension`；自定义安装时以二向箔显示的目录为准。随后点击二向箔里的「允许连接」，在两分钟内打开浏览器扩展并完成一键配置。

以后桌面升级会更新同一目录的扩展文件，扩展在任务完成且弹窗关闭后空闲重载，已打开的视频页需刷新。若之前加载了另一份扩展副本，请先改为当前安装目录；没有自重载能力的旧扩展需要手动重载一次。此更新方式不依赖 Chrome 商店。

## Agent 控制

「设置 → Agent 控制」提供完整或只读 MCP 配置，可连接用户的 Agent。安装包随附 CLI，可管理文稿、任务与队列，也可配置模型和转写提示词。保持二向箔运行，驻留托盘时同样可连接；操作结果与应用中的编辑同步。

## 更新渠道

正式版 **1.1.0**：[下载](https://github.com/Ansel-Poiesis/shengjian-releases/releases/tag/v1.1.0-formal) · [更新说明](releases/1.1.0-formal.md)。测试版 **1.3.4**：[下载](https://github.com/Ansel-Poiesis/shengjian-releases/releases/tag/v1.3.4) · [测试说明](releases/1.3.4.md)。历史测试版 [1.2.0](https://github.com/Ansel-Poiesis/shengjian-releases/releases/tag/v1.2.0) 保留。默认更新仅跟随正式版；测试版需要主动选择，不进入正式版的默认更新通知。

历史 `v1.1.0` 为旧测试发行，保留原有记录。当前正式版使用唯一标签 `v1.1.0-formal`；从旧 1.1.0 测试版切换时，请手动重载浏览器扩展一次，再刷新视频页。每次发行均附 `SHA256SUMS.txt`，可用 PowerShell 的 `Get-FileHash -Algorithm SHA256 文件路径` 校验。

应用中的「设置 → 关于 → 通知与更新」可查看更新记录。问题反馈请提交到 [Issues](https://github.com/Ansel-Poiesis/shengjian-releases/issues)，附版本、系统与复现步骤。

@玩家川行出品
