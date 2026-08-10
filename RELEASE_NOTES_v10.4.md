# ClipStow v10.4 Release Notes

## 主要变化

- 新增小红书图文、视频封面与视频的混合媒体发现、筛选和逐项选择。
- 新增 Behance 正文图片、Vimeo/YouTube 嵌入与 Adobe CCV 媒体发现。
- selection modal 使用固定白底预览区；图片优先使用低分辨率预览，Vimeo 可使用受限公共封面预览。
- 只有小复选框改变选择；文字区只触发预览；保留全选、全不选、按类型互斥和“仅选择此项”。
- 单项失败不会删除已经成功的文件，并显示成功、失败和跳过摘要。
- 保持 B站、YouTube、直接 Vimeo、旧设置以及本机加密登录会话兼容。

## 下载文件

- `ClipStow-10.4-Setup-20260810.exe`
  - 大小：78,833,549 bytes
  - SHA-256：`CED7163A3296E4481EC31D2D5CA821BC8B8C3BF5DE227CBAEBA0B38186BF348B`
- `ClipStow-10.4-Portable-20260810.zip`
  - 大小：106,078,763 bytes
  - SHA-256：`44343C196DBDB4775FA3FAD3CD556519D1CED84D7218E9825CE94FF547832D58`
- `ClipStow-10.4-ThirdParty-Licenses-20260810.zip`
  - 大小：66,011 bytes
  - SHA-256：`A9420429161AB67354892C96349340A97DD1EFD4628659C050FFB467C8809FB5`
  - 内容：README 与本机构建环境可直接取得的第三方许可证全文，不含源码、构建脚本或用户数据。

## 版本、安全与兼容边界

- GUI 版本为 v10.4；Windows FileVersion/ProductVersion 均为 `10.4.0.0`。
- 受保护发布包不包含核心 Python 源码、用户设置、登录会话、日志或下载内容。
- Setup 与主 EXE 的 Authenticode 状态均为 `NotSigned`；请只从官方 GitHub Releases 下载并核对 SHA-256。
- 安装、卸载和升级继续保留用户自己的 `settings.json`，并与既有本机加密登录会话标识兼容。
- 下载能力依赖来源平台、公开链接状态、网络环境与账号权限；单个外部样本失败不代表所有同类链接都可或都不可下载。

第三方组件、许可和源码入口见 `THIRD_PARTY_NOTICES.md` 与许可证附件。
