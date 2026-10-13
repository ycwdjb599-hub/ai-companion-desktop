# 下载、安装与更新 / Install and update

[下载 Windows 安装程序](https://github.com/ycwdjb599-hub/ai-companion-desktop/releases/latest/download/AICompanionTrial-win-Setup.exe) · [版本列表](https://github.com/ycwdjb599-hub/ai-companion-desktop/releases)

## 首次使用

1. 下载 `AICompanionTrial-win-Setup.exe` 并运行。GitHub 的 **Code → Download ZIP** 只会下载此仓库的文档，不是安装程序。
2. 选择程序安装位置。首次打开选择资源盘，点「准备并继续」。程序会自动下载基础资源并校验，不需要手工下载或拼接分块。
3. 同时配置自己的千问 Character Key 和同一业务空间的 ID：[简体中文](SETUP.zh-CN.md) · [繁體中文](SETUP.zh-TW.md) · [English](SETUP.en.md) · [日本語](SETUP.ja.md)。默认业务空间可以使用。
4. 准备完成后点「开始陪伴」。如果只有动作准备失败，可先开始使用，之后到 **右键人物 → 设置 → 人物与动作 → 管理动作资源** 补齐。待机和说话动作互不阻塞。

应用界面当前为简体中文。不需要自行安装 Unity 编辑器、Python、Conda、Git 或 CUDA 工具包；部分重型动作功能需要兼容的 NVIDIA GPU 和驱动。

## 下载失败

- 网络中断后重新准备会续传已有进度。基础资源的分块由程序处理；不要自己改名或拼接。
- 新渠道使用 GitHub，不再依赖原来停用的北京 OSS。动作的 PyTorch/Python 依赖继续使用已冻结的清华、上海交大镜像。
- 原作者的待机动画从其官方 GitHub 下载，不镜像受限动画。它和基础资源、说话动作的下载状态独立。
- GitHub 在部分中国大陆网络可能不可达。若网页或资源链接打不开，请稍后换可用网络；本版本没有承诺所有网络免 VPN 可用。
- 新版显示资源准备失败时，不需要先删除旧资源。保留相同保存位置，校验通过的资源会复用。

## 已安装旧版

退出 AI伴侣，再运行新版安装程序。保持原资源与资料目录；API 配置、聊天和记忆不需要重新填写或重建。基础组件版本仍为 `2026.10.7.1`，完整已安装的约 2108 MiB 基础组件不会因为更换下载渠道而重下。

程序仍在运行或第一次下载未完成时，不会自行替换成新版。应用目前可从本地更新包更新；线上新版本以本仓库 Releases 为准。

## 卸载

右键人物打开设置，在应用更新页选择卸载并确认；也可以使用 Windows 设置 → 应用 → AI伴侣 → 卸载。卸载程序和快捷方式后，聊天、记忆、API 配置与已下载资源会保留。删除这些资料需自行明确选择，卸载不会代你删除。

## English

Download and run **AICompanionTrial-win-Setup.exe** from Releases. The repository ZIP is documentation, not an installer. On first launch, select a resource drive and start preparation. The app downloads and verifies its own resource parts; no manual joining is required. Follow the [English illustrated API guide](SETUP.en.md), then start the companion.

Animation preparation is independent from core chat. Once core resources and your API are ready, you can start and finish missing animations later. Optional motion uses GitHub and pinned Tsinghua/SJTUG mirrors; connectivity depends on your network.

To update, exit the app and run the new installer while retaining the existing data/resource locations. API settings, history and memory stay local. The unchanged base component version is reused when already installed. To uninstall, use the app’s uninstall action or Windows Apps settings; personal data and downloaded resources are retained.

The app UI is currently Simplified Chinese. Windows x64 is supported; GPU features require a compatible NVIDIA GPU/driver. If you report a problem, include the app version and a redacted screenshot, not your API key or private chat database.
