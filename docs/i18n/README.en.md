<p align="center"><img src="../../assets/hero-image.png" alt="AI Companion" width="100%"></p>

<h1 align="center">AI Companion</h1>
<p align="center"><strong>A little company on your Windows desktop.</strong><br>Windows 10 / 11 · x64 · Free preview · Bring your own API key</p>
<p align="center">[简体中文](../../README.md) · [繁體中文](../../docs/i18n/README.zh-TW.md) · [English](../../docs/i18n/README.en.md) · [日本語](../../docs/i18n/README.ja.md)</p>

<p align="center"><a href="https://github.com/ycwdjb599-hub/ai-companion-desktop/releases/latest/download/AICompanionTrial-win-Setup.exe"><strong>↓ Download for Windows</strong></a> · <a href="https://github.com/ycwdjb599-hub/ai-companion-desktop/releases/latest">Releases and changelog</a> · <a href="https://github.com/ycwdjb599-hub/ai-companion-desktop/issues/new/choose">Report a problem</a></p>

A desktop companion you can talk to. Text, voice and an animated character share one experience, while your chat history and memory stay on your computer.

## Three steps to your first conversation

1. Download and run **AICompanionTrial-win-Setup.exe**. Choose an installation location.
2. On first launch, choose a resource drive and click **准备并继续** (Prepare and continue). Resources download automatically. Follow the illustrated guide to enter your **Qwen Character API key and Workspace ID**, then click **检查并继续** (Check and continue).
3. Click **开始陪伴** (Start). Right-click the character for settings. Hold **Right Ctrl** to speak, use **Ctrl + Alt + V** for continuous voice, and **Esc** to stop playback. Shortcuts are configurable.

[Illustrated Qwen setup](../../docs/SETUP.en.md) · [Install, update and troubleshoot](../../docs/INSTALL.md)

## Make yourself at home

- **Desktop presence**: move the character to a taskbar or window edge. Closing settings keeps your companion running.
- **Text and voice**: push-to-talk, continuous listening and a button to interrupt playback. Qwen Character and cloud voice are recommended; local TTS weights are not required.
- **Local continuity**: chat history and memory stay on your PC, with a conversation-history viewer.
- **Your own preferences**: draggable captions with scrolling or sentence mode; adjustable fonts, colors, character size, FPS, rendering quality and animation switches.

<p align="center"><img src="../../assets/model02-desktop.png" alt="Desktop character" width="360"></p>

## Before you download

- The installer contains the app and smaller resources. The initial base download is approximately **2.1 GiB**. Full speech motion adds approximately **4.7 GiB** plus extraction space. Keep **25 GB** free on the resource drive for the full setup.
- Animation modules are optional and prepared separately. Once core chat, memory and your API are ready, use the option to start now and complete animations later.
- An NVIDIA GPU and 16–32 GB RAM are recommended. 8 GB VRAM is a target, not a fully verified minimum. Cloud voice and disabling heavier motion reduce local load.
- The app is free; your chosen API provider bills usage. Necessary conversation context is sent to that provider. The database stays local and keys are encrypted for the current Windows user.
- **These docs support four languages; the Windows UI is currently Simplified Chinese.** Conversation and voice language support depends on the selected provider.
- GitHub may be slow or blocked on some mainland China networks. Motion also uses the original creator’s GitHub and Tsinghua/SJTUG mirrors. Availability without a VPN is not guaranteed everywhere. Downloads support resuming and integrity checks.
- This is a preview without a commercial code-signing certificate. Get installers only from this repository’s Releases. Check the source if Windows blocks a file; do not disable system protection.

A public home for downloads and feedback. Private development material and user conversations are not published here.

[Third-party notices](../../docs/THIRD_PARTY.md) · [Privacy](../../docs/PRIVACY.md)

Inspired by [Project AIRI](https://github.com/moeru-ai/airi) and [Mate Engine](https://github.com/shinyflvre/Mate-Engine). Original illustration and a real Model 2 renderer screenshot; third-party assets retain their own permissions.
