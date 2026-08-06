# 第三方组件通知

ClipStow v10.3 的 Windows 分发包包含或依赖下列第三方组件。版本和许可标识来自本次实际 PYZ 根模块、分发树、本机构建环境及二进制输出；这是一份工程审计记录，不是法律意见。ClipStow 的非开源权利说明不覆盖、缩减或替代任何第三方许可证授予的权利。

本地 Release 附件 `ClipStow-10.3-ThirdParty-Licenses-20260807.zip` 收录了本机构建环境可直接取得的许可证全文。

## 实际运行时 Python 组件

| 组件 | 版本 | 许可 | 官方源码 |
|---|---:|---|---|
| bottle | 0.13.4 | MIT | [bottlepy/bottle](https://github.com/bottlepy/bottle) |
| certifi | 2026.7.22 | MPL-2.0 | [certifi/python-certifi](https://github.com/certifi/python-certifi) |
| cffi | 2.1.1 | MIT-0 | [python-cffi/cffi](https://github.com/python-cffi/cffi) |
| clr_loader | 0.3.1 | MIT | [pythonnet/clr-loader](https://github.com/pythonnet/clr-loader) |
| curl_cffi | 0.15.0 | MIT | [lexiforest/curl_cffi](https://github.com/lexiforest/curl_cffi) |
| packaging | 26.3 | Apache-2.0 OR BSD-2-Clause | [pypa/packaging](https://github.com/pypa/packaging) |
| Pillow | 12.0.0 | MIT-CMU | [python-pillow/Pillow](https://github.com/python-pillow/Pillow) |
| proxy_tools | 0.1.0 | MIT | [jtushman/proxy_tools](https://github.com/jtushman/proxy_tools) |
| pycparser | 3.0 | BSD-3-Clause | [eliben/pycparser](https://github.com/eliben/pycparser) |
| pythonnet | 3.1.0 | MIT | [pythonnet/pythonnet](https://github.com/pythonnet/pythonnet) |
| qrcode | 8.2 | BSD-3-Clause | [lincolnloop/python-qrcode](https://github.com/lincolnloop/python-qrcode) |
| setuptools | 83.0.0 | MIT | [pypa/setuptools](https://github.com/pypa/setuptools) |
| typing_extensions | 4.16.0 | PSF-2.0 | [python/typing_extensions](https://github.com/python/typing_extensions) |
| pywebview | 6.2.1 | BSD-3-Clause | [r0x0r/pywebview](https://github.com/r0x0r/pywebview) |
| yt-dlp | 2026.7.4 | Unlicense | [yt-dlp/yt-dlp](https://github.com/yt-dlp/yt-dlp) |
| yt-dlp-ejs | 0.8.0 | Unlicense AND MIT AND ISC | [yt-dlp/ejs](https://github.com/yt-dlp/ejs) |

除 `proxy_tools` 外，上表组件的实际发行元数据均提供了许可证文件，并已收入许可证附件。`proxy_tools 0.1.0` 的本机发行元数据标识为 MIT，但未附许可证文件；本通知保留其官方源码链接，不据此作超出元数据的法律保证。

## 捆绑运行时与工具

| 组件 | 本次版本/状态 | 工程处理与官方依据 |
|---|---|---|
| Python | 3.11.8，PSF-2.0 | 本机 `LICENSE.txt` 已收入许可证附件；[Python 3.11 许可历史](https://docs.python.org/3.11/license.html) |
| Tcl/Tk | 8.6，permissive | 分发树的 `license.terms` 已收入许可证附件 |
| PyInstaller bootloader | 6.21.0，GPL-2.0-or-later with bootloader exception | 本机 `COPYING.txt` 已收入许可证附件；特殊例外允许用 bootloader 分发非自由程序，仍保留原许可证文本 |
| Deno | 2.8.3，MIT | [denoland/deno 源码与许可](https://github.com/denoland/deno) |
| FFmpeg | 6.0 `essentials_build-www.gyan.dev`，GPL-3.0-or-later | `ffmpeg -L` 与构建配置均确认 GPL v3 or later；[FFmpeg legal](https://ffmpeg.org/legal.html)、[Gyan builds 与源码链接](https://www.gyan.dev/ffmpeg/builds/) |
| NSIS | 3.12，zlib/libpng；所含 LZMA 为 CPL-1.0 | [NSIS License](https://nsis.sourceforge.io/License) |
| Microsoft WebView2 Bootstrapper / Loader | Bootstrapper 1.3.251.21；Loader 随 pywebview 运行 | [WebView2 分发说明](https://learn.microsoft.com/en-us/microsoft-edge/webview2/concepts/distribution)、[Microsoft.Web.WebView2 包与许可](https://www.nuget.org/packages/Microsoft.Web.WebView2) |

FFmpeg 是由 ClipStow 作为独立进程调用的独立 GPLv3-or-later 程序。ClipStow 的非开源声明不适用于 FFmpeg；分发时必须保留 GPLv3-or-later 通知，并通过上方 Gyan 与 FFmpeg 链接提供对应许可和源码获取入口。

## 通知义务的工程落实

- MIT、MIT-0、MIT-CMU、BSD、PSF、Unlicense、Tcl/Tk 与 PyInstaller：在许可证附件中保留本机发行包提供的版权与许可文本。
- `packaging`：保留发行包提供的 Apache-2.0 与 BSD-2-Clause 双许可文本，不替用户选择许可。
- `certifi`：保留 MPL-2.0 全文和官方源码入口；若以后修改受 MPL 覆盖文件，必须重新核对相应源码提供义务。
- FFmpeg、Deno、NSIS 与 WebView2：本机分发树未提供可直接汇总的完整上游许可包，许可证附件 README 保留上表官方许可、源码或分发条款链接。
- 专利授权范围、商标使用和面向特定司法辖区的合规结论不在本次工程审计范围内。

## 仅用于构建

Cython 3.2.9（Apache-2.0）和 PyInstaller hooks 仅用于生成发布包；完整构建工具、项目源码和构建脚本不包含在 Release assets 中。
