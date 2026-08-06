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

## 已知限制与发布门禁

- v10.3 本版决定暂不进行 Authenticode 代码签名；请使用下方 SHA-256 或 `SHA256SUMS.txt` 核对文件完整性。
- 第三方许可全文和通知义务仍有待核实项，尤其是本次 FFmpeg 构建。
- 为保留用户当前安装，卸载及卸载后设置保留回归尚未执行。

第三方许可和卸载回归门禁完成前，本文件和 assets 仅作为本地发布暂存；后续 GitHub Release 必须保持 Draft，不得公开发布。
