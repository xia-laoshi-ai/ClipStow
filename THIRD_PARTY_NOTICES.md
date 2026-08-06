# 第三方组件通知

ClipStow v10.3 的 Windows 分发包包含或依赖下列第三方组件。版本和许可标识来自本次实际构建环境、分发树元数据及项目依赖记录；本文件是发布前清单，不是法律意见。

## 本机元数据已确认

| 组件 | 版本 | 本机元数据中的许可标识 |
|---|---:|---|
| Pillow | 12.0.0 | MIT-CMU |
| PyInstaller bootloader | 6.21.0 | GPL-2.0-or-later，并带允许分发非自由程序的特殊例外 |
| pythonnet | 3.1.0 | MIT |
| pywebview | 6.2.1 | BSD-3-Clause |
| qrcode | 8.2 | BSD（具体文本待核实） |
| yt-dlp | 2026.7.4 | Unlicense |
| yt-dlp-ejs | 0.8.0 | Unlicense AND MIT AND ISC |
| curl_cffi | 0.15.0 | MIT |
| certifi | 2026.7.22 | MPL-2.0 |
| setuptools | 83.0.0 | MIT |
| cffi | 2.1.1 | MIT-0 |
| pycparser | 3.0 | BSD-3-Clause |
| typing_extensions | 4.16.0 | PSF-2.0 |

`clr_loader 0.3.1` 和 `pyinstaller-hooks-contrib 2026.6` 的本机元数据未给出可直接采用的许可标识，必须在公开发布前从对应官方发行源核实。

## 外部运行时与二进制

| 组件 | 本次版本/状态 | 发布前仍需完成 |
|---|---|---|
| Python / Tcl/Tk | Python 3.11.8、Tcl/Tk 8.6 | 核对并随发布材料保留官方许可全文及通知 |
| Deno | 2.8.3 x64 | 从官方发行源核对许可全文与再分发要求 |
| FFmpeg | 6.0 essentials；构建启用 GPL 与 version3 选项 | 核对该具体构建的 GPL 版本、对应源码提供义务和完整许可文本；这是公开发布阻塞项 |
| Microsoft WebView2 Bootstrapper / Loader | Bootstrapper 文件版本 1.3.251.21，签名有效 | 核对微软当前再分发条款和应附通知 |
| NSIS | 3.12 | 核对安装器 stub、插件和压缩组件的许可通知 |

## 仅用于构建

Cython 3.2.9（Apache-2.0）和 PyInstaller hooks 用于生成发布包；完整 Cython 包、项目源码和构建脚本不包含在公开 Release assets 中。仍需在最终法律复核时确认生成物相关通知义务。

## 发布门禁

公开发布前必须补齐上述“待核实”项目的官方许可文本、版权通知与必要源码提供方式。ClipStow 的非开源权利说明不能覆盖、缩减或替代任何第三方许可证授予的权利。
