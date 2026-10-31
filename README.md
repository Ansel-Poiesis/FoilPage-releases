# FoilPage

在本机下载与转写视频，将内容整理为可阅读、可编辑的文稿。支持抖音、B 站、YouTube 与本地媒体。

源码在私有仓库维护，本仓库仅提供 Windows 安装包与更新说明。官方发行入口：[Ansel-Poiesis/FoilPage-releases](https://github.com/Ansel-Poiesis/FoilPage-releases)。

项目名称统一为 FoilPage。**最新正式版为 [1.3.2](https://github.com/Ansel-Poiesis/FoilPage-releases/releases/tag/v1.3.2-formal)（2026-10-31）——本地功能登录即用，取消解锁付费**；测试版为 [1.3.5](https://github.com/Ansel-Poiesis/FoilPage-releases/releases/tag/v1.3.5)。

## 安装与首次使用

1. 从 [最新正式版](https://github.com/Ansel-Poiesis/FoilPage-releases/releases/latest) 下载 `FoilPage-Setup-1.3.2.exe` 并安装。支持 Windows 10 1809 及以上、Windows 11 的 64 位系统，无需安装 Python 或 Node.js。
2. 打开 FoilPage，在「准备」依次完成邮箱登录、环境检测与保存目录设置、本地模型下载。
3. 完成准备后进入「任务」。可粘贴视频链接，也可在「导入媒体」拖入本地视频。

安装包包含 CPU 转写所需的运行组件。NVIDIA GPU 加速包为独立可选下载：选择与桌面版本匹配的 GPU 加速包；1.3.2 正式版文件为 `FoilPage-GPU-Pack-1.3.2.zip`，在「准备 → 环境检测 → 安装 GPU 加速包」中选取，完成后重启。CPU 用户无需下载该包。

## 本地使用与云端积分

登录后即可使用本地模型转写，不收取独立软件解锁费，也不扣云端积分。云端整理与标题优化按账户套餐和积分权限执行；自带 API 由对应模型服务商计费。

| 方式 | 金额与额度 | 转写并发 |
| --- | --- | --- |
| 本地模型 | 登录后使用，不耗云端积分 | 1 |
| 标准云端积分 | ¥19.80／500 积分／30 天 | 2 |
| 专业云端积分 | ¥49.80／2000 积分／30 天 | 4 |

云端积分按需单独购买，不自动续费。本地转写与托管云端整理是不同处理路径；开启云端模型或自带 API 时，按界面说明确认相应的数据处理与服务商费用。切换账户不会移动本机视频和文本，云端权益属于对应账户。
## 浏览器扩展

首次打开 FoilPage 的「浏览器」页，点击「打开扩展目录」。在 Chrome／Edge 的扩展管理页启用开发者模式，选择「加载已解压的扩展」，加载该固定目录。

默认目录为 `%LOCALAPPDATA%\Programs\VideoToArticle\browser-extension`；自定义安装时以 FoilPage 显示的目录为准。随后点击 FoilPage 里的「允许连接」，在两分钟内打开浏览器扩展并完成一键配置。

以后桌面升级会更新同一目录的扩展文件，扩展在任务完成且弹窗关闭后空闲重载，已打开的视频页需刷新。若之前加载了另一份扩展副本，请先改为当前安装目录；没有自重载能力的旧扩展需要手动重载一次。此更新方式不依赖 Chrome 商店。

## Agent 控制

「设置 → Agent 控制」提供完整或只读 MCP 配置，可连接用户的 Agent。安装包随附 CLI，可管理文稿、任务与队列，也可配置模型和转写提示词。保持 FoilPage 运行，驻留托盘时同样可连接；操作结果与应用中的编辑同步。

## 更新渠道

正式版/latest 为 **1.3.2**（[v1.3.2-formal](https://github.com/Ansel-Poiesis/FoilPage-releases/releases/tag/v1.3.2-formal)）；测试版为 **1.3.5**（[v1.3.5](https://github.com/Ansel-Poiesis/FoilPage-releases/releases/tag/v1.3.5)）。默认更新仅跟随正式版；测试版需要主动选择，不进入正式版的默认更新通知。此前的 1.3.4、1.2.0 与 1.1.0 发行说明只记录各自当时状态。

`v1.4.0-formal` 已撤回并作废，正式编号为 1.3.2；历史标签与发行资产保留。每次发行均附 `SHA256SUMS.txt`，可用 PowerShell 的 `Get-FileHash -Algorithm SHA256 文件路径` 校验。

应用中的「设置 → 关于 → 通知与更新」可查看更新记录。问题反馈请提交到 [Issues](https://github.com/Ansel-Poiesis/FoilPage-releases/issues)，附版本、系统与复现步骤。

@玩家川行出品
