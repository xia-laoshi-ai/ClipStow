# ClipStow

ClipStow 是面向 Windows x64 的图片与视频下载工具。当前版本为 **v11.0.14**，提供便携桌面程序和浏览器协助扩展。

> ClipStow 可以免费使用，但不是开源软件。官方版本不会要求为 ClipStow 软件本体付费。

## 下载 v11.0.14

- [下载便携 ZIP](https://github.com/xia-laoshi-ai/ClipStow/releases/download/v11.0.14/ClipStow-11.0.14-Portable-DualMode.zip)
- [README_11.0.14.md](https://github.com/xia-laoshi-ai/ClipStow/releases/download/v11.0.14/README_11.0.14.md)
- [SHA256SUMS_11.0.14.txt](https://github.com/xia-laoshi-ai/ClipStow/releases/download/v11.0.14/SHA256SUMS_11.0.14.txt)
- [第三方通知](https://github.com/xia-laoshi-ai/ClipStow/releases/download/v11.0.14/THIRD_PARTY_NOTICES_11.0.14.md)

请完整解压 ZIP 后运行 `ClipStow.exe`，不要脱离目录单独复制 EXE。旧版本仍可在 [Releases](https://github.com/xia-laoshi-ai/ClipStow/releases) 页面查看。

## 桌面下载

打开 `ClipStow.exe`，将公开链接粘贴到输入框，选择清晰度和保存目录后开始下载。需要账号权限的内容可使用程序内独立登录入口。

## 浏览器协助：安装与验证

1. 解压 ZIP，打开 Chrome、Edge 或 360 的扩展管理页并开启开发者模式。
2. 在“加载已解压扩展”中选择 ZIP 内的 `extension` 文件夹。
3. 打开 ClipStow，进入设置→浏览器协助，选择实际使用的浏览器，点击“我已加载，配置并验证”。
4. 向导会配置当前用户的本地连接并打开验证页面。若浏览器没有自动打开，使用“复制验证地址”后在所选浏览器中打开。
5. 看到“本次扩展通信已验证”后即可关闭验证页。没有回应时只显示“未验证：可能未安装、未启用或需重新加载”，回到扩展管理页重新加载后再验证。

验证只确认本次扩展通信，不读取浏览器 profile/Cookie，不静默安装扩展，也不把本地自检或注册成功当作扩展已安装。切换浏览器后需要重新配置并验证；手动复制到另一浏览器不会被当作原浏览器身份认证。

## 浏览器协助：小红书流程

在已加载并验证扩展的当前笔记页点击扩展；扩展从当前页面提取具体图集或视频任务，确认标题和媒体数量后选择保存目录。不会复制浏览器 Cookie、profile 或登录会话。

## 浏览器协助：其它站点 URL 流程

Behance、B站、YouTube、Vimeo、抖音、Instagram、X、TikTok、Pinterest 只发送当前页面 URL 到 ClipStow 窗口。v11.0.14 在同一 Windows 用户下支持从不同 ClipStow 目录复用已有主窗口；普通双击或 URL 入口不会因此构造第二个主窗口。主窗口忙于下载、捕获、恢复或选择时会保护当前任务并返回忙态提示。用户仍需在主窗口核对链接、设置保存位置，再点击“开始下载”。这些站点不复用浏览器登录，也不读取浏览器 Cookie。

从旧版本升级时请关闭旧版、启动 v11.0.14、加载新包中的 `extension` 并在设置中重新连接；旧浏览器映射可能仍指向旧目录。旧版程序与新版同时运行时不保证跨版本单实例，不能用旧版入口代替新包入口。移动目录或更换电脑后也需要重新连接。

## 发布范围与隐私

本版本为 Windows x64 Portable 交付，主程序和 host 未进行 Authenticode 签名。完整 Chrome/Edge/360 真实按钮矩阵、完整图片/视频媒体矩阵、第二台 Windows 和视频号自动识别仍未完成验证；视频号捕获保持实验性和独立门禁，不作为本次发布通过依据。

浏览器协助只发送当前页面所需的媒体任务或 URL，不复制浏览器登录会话到下载器。反馈 Issue 前请移除账号信息、Cookie、Token、请求头、私人路径和视频链接中的签名参数。

这是免费软件，但不是开源软件。第三方通知与许可证随 v11.0.14 便携包提供。

## 反馈与项目文件

问题和功能建议请提交到 [GitHub Issues](https://github.com/xia-laoshi-ai/ClipStow/issues)。安全与隐私说明见 [SECURITY.md](https://github.com/xia-laoshi-ai/ClipStow/blob/main/SECURITY.md)，项目许可证见 [LICENSE.md](https://github.com/xia-laoshi-ai/ClipStow/blob/main/LICENSE.md)。维护者：海派小朋友Leo。
