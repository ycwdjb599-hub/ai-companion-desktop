<h1 align="center">AI Companion</h1>
<p align="center"><strong>デスクトップに、話し相手を。</strong></p>
<p align="center"><a href="../../README.md">简体中文</a> · <a href="../../docs/i18n/README.zh-TW.md">繁體中文</a> · <a href="../../docs/i18n/README.en.md">English</a> · <a href="../../docs/i18n/README.ja.md">日本語</a></p>
<p align="center"><a href="https://github.com/ycwdjb599-hub/ai-companion-desktop/releases/latest"><img src="https://img.shields.io/github/v/release/ycwdjb599-hub/ai-companion-desktop?style=flat-square&amp;color=6379df" alt="Latest release"></a> <img src="https://img.shields.io/badge/Windows-10%20%2F%2011-6379df?style=flat-square" alt="Windows 10 / 11"> <img src="https://img.shields.io/badge/Free-Preview-a086c5?style=flat-square" alt="Free preview"> <img src="https://img.shields.io/badge/API-Bring%20your%20own-74818d?style=flat-square" alt="Bring your own API key"></p>

<p align="center"><a href="https://github.com/ycwdjb599-hub/ai-companion-desktop/releases/latest/download/AICompanionTrial-win-Setup.exe"><img src="../../assets/download-windows.svg" alt="Windows インストーラーをダウンロード" width="272"></a><br><a href="../../docs/SETUP.ja.md">画像付き設定ガイド</a> · <a href="https://github.com/ycwdjb599-hub/ai-companion-desktop/releases/latest">リリース</a> · <a href="https://github.com/ycwdjb599-hub/ai-companion-desktop/issues/new/choose">問題を報告</a></p>

<p align="center"><img src="../../assets/hero-image.png" alt="AI Companion illustration" width="860"></p>
<p align="center"><a href="#companion">キャラクターと機能</a> · <a href="#technology">技術</a> · <a href="#start">クイックスタート</a> · <a href="#requirements">利用環境</a></p>

Windows のデスクトップに暮らす AI の話し相手。文字や声で今日のことを話せます。会話履歴と記憶は自分の PC に保存されます。

## 0.1.16 · 読みやすいチャット、自然な通話

- **文字・スタンプ・画像**：線画アイコンを統一。送信後は入力欄をすぐに空にし、完成した返信をまとめて表示します。双方のアイコンを変更でき、文字の大きさはチャット設定で調整できます。
- **専用の通話画面**：アイコン、呼び出し、経過時間、終了ボタンを表示。応答・拒否の前に長さの異なる待ち時間があり、キャンセルした通話が後から接続されることはありません。押して話す機能は引き続き利用できます。
- **静かな自発メッセージ**：設定で有効化できます。自発メッセージは読み上げません。未返信なら追加の反応は任意で最大1回、その後は送信を休止します。
- **知り合うところから**：初対面ではすぐに通話に応答しません。実際の交流と現在の関係を参照し、好感度の数値は表示しません。拒否後も文字で会話できます。
- **前回の選択を保存**：初回に確定したモードは再起動後も維持します。変更は設定 → インタラクションとショートカット → 関係モード → アプリモードから行います。

選択した画像は設定済みの画像認識サービスに送信されます。メインの会話モデルを切り替える必要はありません。

基本リソースのバージョンは変更せず、検証済みの既存データを再利用します。変更と検証範囲は [更新履歴](../CHANGELOG.md) を参照してください。

<table><tr><td width="72%"><img src="../../assets/text-chat.png" alt="Text chat" width="780"></td><td width="28%"><img src="../../assets/voice-call.png" alt="Voice call" width="260"></td></tr></table>

<sub>実際の Windows UI。会話文はテスト用で、利用者の私的な会話ではありません。</sub>

既定アバターは **Alpine 16 Daisy** になりました。旧 Model 2 のファイルも復帰用に保持します。大容量の音声駆動モーションはまだ Model 2 専用のため、Alpine 16 ではダウンロードを省略します。基本の文字・音声・表情・待機には不要です。マイク通話全体とビデオメディアは今回再検証していません。

<a name="companion"></a>

## デスクトップで、そばにいる

<table>
<tr>
<td align="center" width="36%"><a href="../../assets/alpine16-avatar.png"><img src="../../assets/alpine16-avatar.png" alt="Alpine 16 runtime portrait" width="240"></a><br><sub>Alpine 16 · 実行モデルのポートレート</sub></td>
<td width="64%">
<p><strong>デスクトップの存在感</strong><br>ドラッグ、タスクバーやウィンドウ端の座り姿勢、待機モーションと表情。</p>
<p><strong>文字と音声</strong><br>文字チャット、押して話す、連続音声。ボタンで応答を中断できます。</p>
<p><strong>会話の続き</strong><br>履歴と記憶を PC に保存。履歴ビューアーで会話を振り返れます。</p>
<p><strong>自分好みの表示</strong><br>移動できる字幕、スクロール・文単位表示。フォント、色、サイズ、FPS、画質を調整。</p>
</td>
</tr>
</table>

<a name="technology"></a>

## 使っている技術

対話と音声合成はクラウド、認識・アバター表示・データ保存は PC で処理します。モーションは独立して準備するため、ダウンロード失敗でも基本チャットを先に利用できます。

| モジュール | 現在の技術 | 役割 |
| --- | --- | --- |
| デスクトップ UI | **C# · .NET 10 · WinForms** | Windows UI と会話処理の統括 |
| アバター表示 | **Unity · UniVRM** | 透明デスクトップアバター、VRM、表情とアニメーション |
| AI 対話 | **Qwen Character · OpenAI-compatible API** | 自分の API キーを使う推奨対話サービス |
| 音声認識 | **SenseVoiceSmall INT8 · sherpa-onnx · Silero VAD** | ローカル音声認識と発話検出 |
| 音声合成 | **Qwen TTS API** | クラウド音声合成。ローカル音声モデルは任意 |
| ローカル記憶 | **SQLite · Qwen3 Embedding 0.6B** | 会話・状態の保存とローカル履歴の意味検索 |
| 発話モーション | **StreamTalk · WavLM · Fixed Body (Model 2)** | 任意の音声駆動モーションとアバター骨格への適用 |
| インストール・配布 | **Velopack · GitHub Releases · SHA-256** | インストール、リソース再開、整合性確認とバージョン配布 |

<details>
<summary>入力・対話・記憶・モーションのつながり</summary>

```mermaid
flowchart TD
  Text["文字入力"]
  Mic["マイク"]
  ASR["ローカル認識"]
  Core["対話とコンテキスト"]
  DB["会話と記憶"]
  LLM["クラウド対話"]
  TTS["クラウド音声"]
  Motion["任意の発話モーション"]
  Avatar["デスクトップアバターと字幕"]
  Text --> Core
  Mic --> ASR --> Core
  Core <--> DB
  Core <--> LLM
  Core --> TTS
  Core --> Avatar
  TTS --> Motion --> Avatar
```

</details>

<a name="start"></a>

## 3 ステップで最初の会話へ

1. **インストール** — 上の Windows インストーラーを実行します。Unity Editor、Python、Conda を手動で導入する必要はありません。
2. **接続** — 保存先を選び 准备并继续（準備して続行）をクリック。リソースは自動取得されます。画像ガイドに沿って Qwen Character キーと Workspace ID を入力し、检查并继续（確認して続行）をクリックします。
3. **開始** — 开始陪伴（開始）をクリック。右クリックで設定を開けます。外観や音声の設定は後からゆっくり調整できます。

[画像付き設定ガイド](../../docs/SETUP.ja.md)

| 操作 | 既定 |
| --- | --- |
| 設定を開く | アバターを右クリック |
| 押して話す | Right Ctrl |
| 連続音声を切り替え | Ctrl + Alt + V |
| 再生を停止 | Esc |

ショートカットは設定で変更できます。

<a name="requirements"></a>

## 利用前に

| 項目 | 説明 |
| --- | --- |
| システム | Windows 10 / 11、x64。アプリ UI は現在、簡体字中国語です。 |
| 接続 | 自分の API キーと GitHub・利用サービスへの接続。アプリは無料、API 料金は提供元が請求します。 |
| 空き容量 | 基本リソースは約 2.1 GiB、完全な発話モーションはさらに約 4.7 GiB。完全な準備には 25 GB の空き容量を推奨。 |
| ローカルモーション | NVIDIA GPU、16–32 GB RAM を推奨。VRAM 8 GB は検証中の目標で、保証済み最低要件ではありません。 |

## ダウンロード・更新・プライバシー

<details>
<summary>モーションの準備に失敗しても開始できますか？</summary>

基本チャット、記憶、API の準備後、先开始使用 · 动作稍后补齐（先に使う）を選べます。待機と発話モーションは独立して準備され、後から追加できます。

</details>

<details>
<summary>既存のインストールを更新するには？</summary>

旧版を終了し、同じデータとリソース保存先を保って新インストーラーを実行します。オンライン版は Releases を確認。アプリはローカル更新パッケージに対応し、GitHub 自動更新はまだ接続していません。

</details>

<details>
<summary>会話とキーはどこに保存されますか？</summary>

会話と記憶は PC に保存。キーは現在の Windows ユーザー向けに DPAPI で暗号化されます。クラウド API にはサービスに必要な文章とコンテキストが送られます。

</details>

<details>
<summary>Windows にインストーラーをブロックされたら？</summary>

商用コード署名はまだありません。このリポジトリの Releases と SHA256SUMS.txt を確認し、システム保護を無効にしないでください。

</details>

[インストール・更新・アンインストール](../../docs/INSTALL.md) · [プライバシー](../../docs/PRIVACY.md) · [第三者ライセンス](../../docs/THIRD_PARTY.md)

---

公開ダウンロード・文書・フィードバック用のリポジトリです。開発ソースは非公開です。

構成の参考：[Project AIRI](https://github.com/moeru-ai/airi) · [Open-LLM-VTuber](https://github.com/Open-LLM-VTuber/Open-LLM-VTuber) · [Mate Engine](https://github.com/shinyflvre/Mate-Engine)。
