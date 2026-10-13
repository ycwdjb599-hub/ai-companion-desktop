<p align="center"><img src="../../assets/hero-image.png" alt="AI Companion" width="100%"></p>

<h1 align="center">AI Companion</h1>
<p align="center"><strong>Windows のデスクトップに、小さな話し相手を。</strong><br>Windows 10 / 11 · x64 · 無料プレビュー · 自分の API キーを使用</p>
<p align="center"><a href="../../README.md">简体中文</a> · <a href="../../docs/i18n/README.zh-TW.md">繁體中文</a> · <a href="../../docs/i18n/README.en.md">English</a> · <a href="../../docs/i18n/README.ja.md">日本語</a></p>

<p align="center"><a href="https://github.com/ycwdjb599-hub/ai-companion-desktop/releases/latest/download/AICompanionTrial-win-Setup.exe"><strong>↓ Windows 版をダウンロード</strong></a> · <a href="https://github.com/ycwdjb599-hub/ai-companion-desktop/releases/latest">リリースと更新内容</a> · <a href="https://github.com/ycwdjb599-hub/ai-companion-desktop/issues/new/choose">不具合を報告</a></p>

文字チャット、音声、デスクトップのキャラクターをひとつにした AI コンパニオン。会話履歴と記憶は自分の PC に保存されます。

## 最初の会話まで、3 ステップ

1. **AICompanionTrial-win-Setup.exe** をダウンロードして実行し、インストール先を選びます。
2. 初回起動でリソースの保存先を選び、**准备并继续**（準備して続行）をクリックします。リソースは自動ダウンロードされます。画像ガイドを見ながら **Qwen Character の API キーと Workspace ID** を入力し、**检查并继续**（確認して続行）をクリックします。
3. **开始陪伴**（開始）をクリックします。キャラクターを右クリックすると設定が開きます。**右 Ctrl** を押して話し、**Ctrl + Alt + V** で連続音声を切り替え、**Esc** で再生を止めます。ショートカットは変更できます。

[画像付き Qwen 設定ガイド](../../docs/SETUP.ja.md) · [インストールとトラブル対策](../../docs/INSTALL.md)

## デスクトップでできること

- **そばにいるキャラクター**：タスクバーやウィンドウの端に移動できます。設定を閉じてもキャラクターは終了しません。
- **文字と音声**：押して話す、連続音声、ボタンで応答を中断。Qwen Character とクラウド音声を推奨し、ローカル TTS は必須ではありません。
- **PC に残る会話**：履歴と記憶はローカルに保存。会話履歴の表示機能もあります。
- **好みに合わせた表示**：移動できる字幕、スクロール・文単位表示、フォントや色、キャラクターサイズ、FPS、画質、アニメーションを調整できます。

<p align="center"><img src="../../assets/model02-desktop.png" alt="Desktop character" width="360"></p>

## ダウンロード前に

- 初回の基本リソースは約 **2.1 GiB**。音声連動モーションにはさらに約 **4.7 GiB** のダウンロードと展開用の空き容量が必要です。完全なセットアップには **25 GB** の空き容量を推奨します。
- モーションは後から追加できます。基本チャット、記憶、API の準備ができたら先に利用を開始できます。待機モーションと音声連動モーションは別々に準備します。
- NVIDIA GPU と 16–32 GB の RAM を推奨。VRAM 8 GB は検証中の目標であり、動作保証済みの最低要件ではありません。クラウド音声や重いモーションの無効化で負荷を軽減できます。
- アプリは無料ですが API 利用料は選んだサービスから請求されます。必要な会話コンテキストはそのサービスに送信されます。DB は PC に保存され、キーは現在の Windows ユーザー向けに暗号化されます。
- **このリポジトリの文書は4言語対応です。Windows UI は現在、簡体字中国語です。** 会話・音声の対応言語はサービスによって異なります。
- この配布版は外部インターネットに接続できる環境を前提とします。アプリのリソースは GitHub、モーションの依存パッケージは公式配布元を利用します。ダウンロードの再開と整合性確認に対応しています。
- 商用コード署名のないプレビュー版です。このリポジトリの Releases から取得し、Windows にブロックされたら入手先を確認してください。システム保護を無効にする必要はありません。

ダウンロードとフィードバック用の公開リポジトリです。非公開の開発資料やユーザーの会話は含みません。

[Third-party notices](../../docs/THIRD_PARTY.md) · [Privacy](../../docs/PRIVACY.md)

Inspired by [Project AIRI](https://github.com/moeru-ai/airi) and [Mate Engine](https://github.com/shinyflvre/Mate-Engine). Original illustration and a real Model 2 renderer screenshot; third-party assets retain their own permissions.
