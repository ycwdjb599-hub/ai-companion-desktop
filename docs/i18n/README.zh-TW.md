<p align="center"><img src="../../assets/hero-image.png" alt="AI伴侶" width="100%"></p>

<h1 align="center">AI伴侶</h1>
<p align="center"><strong>讓她坐在你的桌面上，聊聊今天。</strong><br>Windows 10 / 11 · 64 位元 · 免費預覽版 · 自備 API Key</p>
<p align="center"><a href="../../README.md">简体中文</a> · <a href="../../docs/i18n/README.zh-TW.md">繁體中文</a> · <a href="../../docs/i18n/README.en.md">English</a> · <a href="../../docs/i18n/README.ja.md">日本語</a></p>

<p align="center"><a href="https://github.com/ycwdjb599-hub/ai-companion-desktop/releases/latest/download/AICompanionTrial-win-Setup.exe"><strong>↓ 下載 Windows 安裝程式</strong></a> · <a href="https://github.com/ycwdjb599-hub/ai-companion-desktop/releases/latest">版本與更新說明</a> · <a href="https://github.com/ycwdjb599-hub/ai-companion-desktop/issues/new/choose">回報問題</a></p>

常駐 Windows 桌面的 AI 夥伴，把文字、語音與桌面人物放在一起，聊天與記憶保留在你的電腦。

## 三步開始第一次聊天

1. 下載並執行 **AICompanionTrial-win-Setup.exe**，選擇安裝位置。
2. 首次開啟後選擇資源磁碟，按 **准备并继续**。基礎資源自動下載；依圖文指引填入自己的 **千問 Character API Key 與業務空間 ID**，按 **检查并继续**。
3. 準備好後按 **开始陪伴**。右鍵人物開啟設定；按住 **右 Ctrl** 說話、**Ctrl + Alt + V** 切換連續語音，**Esc** 停止播放。快捷鍵可以修改。

[看圖設定千問](../../docs/SETUP.zh-TW.md) · [安裝與常見問題](../../docs/INSTALL.md)

## 桌面上的陪伴

- **桌面人物**：拖到工作列或視窗邊緣坐下；關閉設定不會退出人物。
- **文字與語音**：按住說話、連續語音與手動打斷。預設推薦千問 Character 與雲端語音，不必先下載本機 TTS。
- **本機記憶**：聊天與記憶保留在電腦，可查看對話歷史。
- **自由調整**：拖動字幕、逐句或捲動顯示，調整字型、顏色、人物大小、FPS、畫質與動作。

<p align="center"><img src="../../assets/model02-desktop.png" alt="Desktop character" width="360"></p>

## 下載前請留意

- 首次基礎資源約 **2.1 GiB**；完整說話動作另需約 **4.7 GiB** 下載與解壓縮空間。建議資源磁碟保留 **25 GB**。
- 基礎聊天、記憶與 API 準備好後，可先開始使用，再補下載動作；待機與說話動作各自準備。
- 建議 NVIDIA 獨立顯示卡、16–32 GB 記憶體。8 GB 顯示記憶體是尚待全面驗證的目標；雲端語音和停用重型動作可降低負載。
- 軟體免費，外部 API 由供應商向你計費。必要上下文會傳送給所選服務；資料庫留在本機，Key 以目前 Windows 使用者加密儲存。
- **此倉庫文件提供四種語言；Windows 介面目前為簡體中文。** 對話及配音語言支援取決於服務。
- 本版本以可連線外網的環境為前提。程式資源由 GitHub 提供，動作依賴使用官方來源；支援續傳與校驗。
- 目前是未具商業程式碼簽章的預覽版。僅從本倉庫 Releases 下載；系統攔截時先檢查來源，不必關閉防護。

公開下載與回報入口；不包含私人研發資料或使用者聊天紀錄。

[Third-party notices](../../docs/THIRD_PARTY.md) · [Privacy](../../docs/PRIVACY.md)

Inspired by [Project AIRI](https://github.com/moeru-ai/airi) and [Mate Engine](https://github.com/shinyflvre/Mate-Engine). Original illustration and a real Model 2 renderer screenshot; third-party assets retain their own permissions.
