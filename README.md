# ClipStow

ClipStow 是面向 Windows x64 的图片与视频下载工具。当前版本为 **v11.0.16**，提供便携桌面程序和浏览器协助扩展。

> ClipStow 可以免费使用，但不是开源软件。官方版本不会要求为 ClipStow 软件本体付费。

## 下载 v11.0.16

- [下载便携 ZIP](https://github.com/xia-laoshi-ai/ClipStow/releases/download/v11.0.16/ClipStow-11.0.16-Portable-DualMode.zip)
- [README_11.0.16.md](https://github.com/xia-laoshi-ai/ClipStow/releases/download/v11.0.16/README_11.0.16.md)
- [SHA256SUMS_11.0.16.txt](https://github.com/xia-laoshi-ai/ClipStow/releases/download/v11.0.16/SHA256SUMS_11.0.16.txt)
- [第三方通知](https://github.com/xia-laoshi-ai/ClipStow/releases/download/v11.0.16/THIRD_PARTY_NOTICES_11.0.16.md)

请完整解压 ZIP 后运行 `ClipStow.exe`，不要脱离目录单独复制 EXE。旧版本仍可在 [Releases](https://github.com/xia-laoshi-ai/ClipStow/releases) 页面查看。

## 桌面下载

打开 `ClipStow.exe`，将公开链接粘贴到输入框，选择清晰度和保存目录后开始下载。需要账号权限的内容可使用程序内独立登录入口。

## 浏览器协助：安装与验证

1. 解压 ZIP，打开 Chrome、Edge 或 360 的扩展管理页并开启开发者模式。
2. 在“加载已解压扩展”中选择 ZIP 内的 `extension` 文件夹。
3. 打开 ClipStow，进入设置→浏览器协助，选择实际使用的浏览器，点击“我已加载，配置并验证”。
4. 向导会配置当前用户的本地连接并打开验证页面。看到“本次扩展通信已验证”后即可关闭验证页。

验证只确认本次扩展通信，不读取浏览器 profile/Cookie，不静默安装扩展，也不把本地自检或注册成功当作扩展已安装。切换浏览器后需要重新配置并验证。升级时请关闭旧版、解压新包、重新加载新包中的 `extension`，再在设置中重新连接；旧 native-host 映射可能仍指向旧目录。

## Vimeo 与 Behance

Vimeo 播放器媒体协助只在用户点击扩展并授予 `https://player.vimeo.com/*` 权限后运行；它读取公开播放器配置，核对视频 ID 与允许的 HTTPS HLS CDN，再通过现有本地连接交给桌面端下载。浏览器协助不导出 Cookie 或登录资料，公开材料不记录媒体临时签名参数。

Behance 项目建议先完成页面刷新，再点击扩展；扩展可把真实图片/视频列表交给桌面端逐项选择，覆盖混合媒体、动画 GIF 和 Adobe CCV 样本。普通粘贴入口仍可能受到站点 403 影响。

## 小红书流程

在已加载并验证扩展的当前笔记页点击扩展；扩展从当前页面提取具体图集或视频任务，确认标题和媒体数量后选择保存目录。不会复制浏览器 Cookie、profile 或登录会话。

其它站点 URL 仍发送当前页面 URL 到已有 ClipStow 窗口；主窗口忙碌时保护当前任务，不创建第二个主窗口。隐藏或最小化窗口会尝试恢复到前台，但 Windows 前台锁可能拒绝激活；程序不永久置顶。用户仍需在主窗口核对链接并点击“开始下载”。

## 发布范围与隐私

本版本为 Windows x64 Portable 交付，主程序和 host 未进行 Authenticode 签名。完整 Chrome/Edge/360 真实按钮矩阵、第二台 Windows、所有站点完整媒体矩阵和视频号自动识别仍未完成验证；视频号保持实验性和独立门禁。

浏览器协助不复制浏览器登录会话到下载器。反馈 Issue 前请移除账号信息、Cookie、Token、请求头、私人路径和视频链接中的签名参数。

这是免费软件，但不是开源软件。第三方通知与许可证随 v11.0.16 便携包提供。

问题和功能建议请提交到 [GitHub Issues](https://github.com/xia-laoshi-ai/ClipStow/issues)。项目许可证见 [LICENSE.md](https://github.com/xia-laoshi-ai/ClipStow/blob/main/LICENSE.md)。
