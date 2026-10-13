<p align="center"><img src="assets/hero-image.png" alt="AI伴侣" width="100%"></p>

<h1 align="center">AI伴侣</h1>
<p align="center"><strong>让她坐在你的桌面上，和你说说今天。</strong><br>Windows 10 / 11 · 64 位 · 免费预览版 · 自备 API Key</p>
<p align="center">[简体中文](README.md) · [繁體中文](docs/i18n/README.zh-TW.md) · [English](docs/i18n/README.en.md) · [日本語](docs/i18n/README.ja.md)</p>

<p align="center"><a href="https://github.com/ycwdjb599-hub/ai-companion-desktop/releases/latest/download/AICompanionTrial-win-Setup.exe"><strong>↓ 下载 Windows 安装程序</strong></a> · <a href="https://github.com/ycwdjb599-hub/ai-companion-desktop/releases/latest">查看版本与更新说明</a> · <a href="https://github.com/ycwdjb599-hub/ai-companion-desktop/issues/new/choose">反馈问题</a></p>

一个常驻 Windows 桌面的 AI 小伙伴。文字聊天、语音交流和桌面人物放在一起，相处记录留在你的电脑里。

## 从下载到第一次聊天，只需三步

1. 下载并运行 **AICompanionTrial-win-Setup.exe**，保留默认程序目录或选择自己的位置。
2. 首次打开后选择资源保存盘，点击 **准备并继续**。基础资源自动下载；同时按图文指引配置自己的 **千问 Character API Key 和业务空间 ID**，点击 **检查并继续**。
3. 准备完成后点击 **开始陪伴**。右键人物打开设置，按住 **右 Ctrl** 说话；连续语音用 **Ctrl + Alt + V**，**Esc** 停止播放。快捷键可修改。

[看图配置千问](docs/SETUP.zh-CN.md) · [安装、升级和常见问题](docs/INSTALL.md)

## 她可以陪你做什么

- **桌面陪伴**：拖动人物，让她坐在任务栏或窗口边缘。关闭设置窗口后人物仍在。
- **想说就说**：文字聊天、按住说话和连续语音；可以用按钮打断回复。默认推荐千问 Character，云端配音无需先下载本地 TTS。
- **延续交流**：聊天记录与记忆保存在本机，可以打开历史记录继续查看。
- **按自己的习惯调整**：字幕支持拖动、滚动或逐句显示，字体与颜色可调；人物大小、帧率、画质和动作开关可设置。

<p align="center"><img src="assets/model02-desktop.png" alt="Desktop character" width="360"></p>

## 开始前，了解这几件事

- 安装包只包含程序和部分小资源。首次基础下载约 **2.1 GiB**；使用完整说话动作还需约 **4.7 GiB** 下载和额外解压空间。建议资源盘预留 **25 GB**。
- 动作是可补齐的可选组件。基础聊天、记忆和 API 准备好后，动作下载失败也可点击 **先开始使用 · 动作稍后补齐**。待机和说话动作分别准备。
- 建议 NVIDIA 独显、16–32 GB 内存；8 GB 显存是目标配置，尚未完成所有设备验证。关闭重型动作或使用云端声音可减轻负担。
- 软件免费，API 调用由你所选服务计费。聊天所需上下文会发送给该服务；聊天数据库保留本地，Key 按当前 Windows 用户加密保存。
- **本仓库文档有四种语言，当前 Windows 界面为中文。** 不同语言的对话和配音支持取决于所选服务。
- GitHub 在部分中国大陆网络可能较慢或不可达。不能保证所有网络无 VPN 可用。动作还会访问原作者 GitHub，以及清华、上海交大镜像；安装程序有续传和校验。
- 当前为预览版，安装程序尚无商业代码签名。只从此仓库的 Releases 获取安装文件。系统拦截时先检查来源；不需要关闭系统防护。

这是公开下载与反馈仓库，不包含私人研发资料或用户聊天记录。

[Third-party notices](docs/THIRD_PARTY.md) · [Privacy](docs/PRIVACY.md)

Inspired by [Project AIRI](https://github.com/moeru-ai/airi) and [Mate Engine](https://github.com/shinyflvre/Mate-Engine). Original illustration and a real Model 2 renderer screenshot; third-party assets retain their own permissions.
