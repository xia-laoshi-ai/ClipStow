# ClipStow v10.3 Release Notes

## 主要变化

- 产品名称和界面版本统一为 ClipStow v10.3。
- 使用 Windows x64 原生扩展保护自研核心；公开包不包含核心 Python 源码或核心 PYZ 字节码。
- 使用快速启动的 onedir 结构，提供安装版和便携 ZIP。
- 修复 YouTube 独立登录窗口关闭后的状态识别，并验证关闭软件、重新启动后的本机会话恢复。
- 安装器默认目录统一为 `Programs\ClipStow`，支持用户级自定义目录安装。
- 快速使用说明位于主窗口右上角 `?`。

## 下载文件

- `ClipStow-10.3-Setup-20260807.exe`
  - 大小：78,683,788 bytes
  - SHA-256：`8BE1198D95734E8D1A59F8C1299A13323FFF1EB5BCED2F026877645A2ADE110E`
- `ClipStow-10.3-Portable-20260807.zip`
  - 大小：105,847,703 bytes
  - SHA-256：`69310506B51E538D25AFC0B8AA81D3EAC08237C56A301E6DF5765904AE17AE88`
- `ClipStow-10.3-ThirdParty-Licenses-20260807.zip`
  - 大小：66,011 bytes
  - SHA-256：`2B86D343B4A03329C80A9C271D80DFE0CD84D68B4BA86BD762C5118FDAC9504F`
  - 内容：README 与本机构建环境可直接取得的第三方许可证全文，不含源码、构建脚本或用户数据。

## 已知限制与发布状态

- v10.3 本版决定暂不进行 Authenticode 代码签名；请使用下方 SHA-256 或 `SHA256SUMS.txt` 核对文件完整性。
- 第三方许可工程审计已完成；FFmpeg 作为独立 GPLv3-or-later 程序披露，许可与源码入口见 `THIRD_PARTY_NOTICES.md` 和许可证附件。
- v2 卸载、设置保留、重装、真实 GUI 和本机会话保留回归已完成。

当前变更仅完成本地发布暂存；GitHub Release 仍保持 Draft，尚未上传许可证附件或执行 publish。
