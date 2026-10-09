# ClipStow

ClipStow 是面向 Windows x64 的图片与视频下载工具。当前版本为 **v11.0.12**，提供便携桌面程序和浏览器协助扩展。

> ClipStow 可以免费使用，但不是开源软件。官方版本不会要求为 ClipStow 软件本体付费。

## 下载 v11.0.12

- [下载便携 ZIP](https://github.com/xia-laoshi-ai/ClipStow/releases/download/v11.0.12/ClipStow-11.0.12-Portable-DualMode.zip)
- [README_11.0.12.md](https://github.com/xia-laoshi-ai/ClipStow/releases/download/v11.0.12/README_11.0.12.md)
- [SHA256SUMS_11.0.12.txt](https://github.com/xia-laoshi-ai/ClipStow/releases/download/v11.0.12/SHA256SUMS_11.0.12.txt)
- [第三方通知](https://github.com/xia-laoshi-ai/ClipStow/releases/download/v11.0.12/THIRD_PARTY_NOTICES_11.0.12.md)

请完整解压 ZIP 后运行 `ClipStow.exe`，不要脱离目录单独复制 EXE。旧版本仍可在 [Releases](https://github.com/xia-laoshi-ai/ClipStow/releases) 页面查看。

## 桌面下载

打开 `ClipStow.exe`，将公开链接粘贴到输入框，选择清晰度和保存目录后开始下载。需要账号权限的内容可使用程序内独立登录入口。

## 浏览器协助：小红书流程

1. 解压 ZIP，打开浏览器扩展管理页并开启开发者模式。
2. 在 Chrome、Edge 或 360 中加载 ZIP 内的 `extension` 文件夹。
3. 打开 `ClipStow.exe`，进入设置→浏览器协助，选择浏览器并点击连接。
4. 回到小红书当前笔记页点击扩展；扩展从当前页面提取具体图集或视频任务，确认标题和媒体数量后选择保存目录。不会复制浏览器 Cookie、profile 或登录会话。

## 浏览器协助：其它站点 URL 流程

Behance、B站、YouTube、Vimeo、抖音、Instagram、X、TikTok、Pinterest 只发送当前页面 URL 到 ClipStow 窗口。已有主窗口时复用该窗口；用户核对链接和保存位置后，仍需点击“开始下载”。这些站点不复用浏览器登录，也不读取浏览器 Cookie。

移动目录或更换电脑后重新连接，不要复制浏览器登录会话。升级旧版时关闭旧版、启动 v11.0.12，进入设置→浏览器协助→选择浏览器→点击“一键连接”，并重新加载新包中的扩展；仅重新加载扩展不会更新旧浏览器连接映射，旧版扩展映射仍指向旧程序。扩展点击时会复用已有主窗口，下载或捕获忙碌时保护当前任务。首次使用仍需加载 ZIP 内的扩展并完成程序内一键连接。下载完成后，主窗口底部左侧可查看下载结果，右侧可打开实际下载文件夹；小红书完成窗关闭后可继续使用扩展。

## 发布说明

完整更新说明见 [v11.0.12 Release](https://github.com/xia-laoshi-ai/ClipStow/releases/tag/v11.0.12)。

## 范围与隐私

扩展点击时会复用已有主窗口并保护忙碌任务；真实浏览器点击、完整媒体矩阵和跨设备验证仍未完成。v11.0.11 已核验桌面最终布局，v11.0.8 曾完成 Edge 连接核验，并收到 Chrome/Edge 用户下载成功反馈。这些事实不代表当前版本已完成跨设备或完整浏览器矩阵。程序未签名。视频号自动识别为实验性功能，保留手动兜底。

浏览器协助通过当前笔记页发送媒体任务，不复制浏览器登录会话到下载器。反馈 Issue 前请移除账号信息、Cookie、Token、请求头、私人路径和视频链接中的签名参数。

这是免费软件，但不是开源软件。第三方通知与许可证随 v11.0.12 便携包提供。

## 反馈与项目文件

问题和功能建议请提交到 [GitHub Issues](https://github.com/xia-laoshi-ai/ClipStow/issues)。安全与隐私说明见 [SECURITY.md](https://github.com/xia-laoshi-ai/ClipStow/blob/main/SECURITY.md)，项目许可证见 [LICENSE.md](https://github.com/xia-laoshi-ai/ClipStow/blob/main/LICENSE.md)。维护者：海派小朋友Leo。
