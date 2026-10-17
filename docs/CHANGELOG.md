# 更新记录 / Release history

## 0.1.16 · 2026-10-17

[下载 Windows 安装程序](https://github.com/ycwdjb599-hub/ai-companion-desktop/releases/download/v0.1.16/AICompanionTrial-win-Setup.exe) · [完整版本资产](https://github.com/ycwdjb599-hub/ai-companion-desktop/releases/tag/v0.1.16)

- 文字输入发送后立即清空；回复在完整交付后一次显示。移除多余的发送、完成和收藏操作提示。
- 统一文字聊天工具栏，支持按住说话、语音通话、彩色表情和图片输入；可更换双方头像、调整聊天字号。
- 主动消息保持静音，独立于普通回复的语音开关。未回复时最多尝试一次可选回应，然后暂停；跨重启保留暂停状态，收到新回复后再按原额度和间隔判断。
- 语音通话使用独立头像界面。等待时间随每次呼叫变化；拒接前通常等待 6–12 秒。取消、拒接和通话结束分别记录，不会取消后又接通。
- 新认识时逐步建立联系意愿，按实际有内容的交流与关系状态判断；不显示好感度数字。普通打字与按住说话不受通话资格限制。
- 首次确认相处模式后保存。后续入口为设置 → 互动与快捷键 → 相处模式 → 应用模式。
- 新安装默认包含 16 号阿尔卑斯雏菊裙装、匹配渲染器和布料配置。旧 Model 2 保留在程序包的 `assets/fallback/Model2.vrm`；已有安装继续使用原先保存的人物路径，不强制覆盖自选人物。

### 使用边界

- 现有大型语音驱动动作组件绑定 Model 2。16 号暂不使用该组件，安装时跳过其下载；基本语音和口型不依赖它。
- 基础资源版本仍为 `2026.10.7.1`，校验有效的已有资源继续复用。受限制的原站动作未重新分发；新安装仍从原作者来源获取。
- 这次没有更换用户已选择的主聊天模型。公共安装从空白用户资料开始，不包含维护者的聊天、正式人生、记忆或凭据。
- 本机原生界面与定向功能检查不代表所有设备都通过；真人麦克风完整通话、完整视频媒体和全项目测试本轮未重跑。软件仍为未做商业代码签名的预览版。

### 更新与恢复

先退出旧版，再运行新版安装程序，保留相同的资料与资源位置。升级前可自行备份资料目录。旧版本的 Releases 继续保留；恢复旧程序不等于回滚聊天或记忆，不删除资料来降级。

### English

Completed text replies now appear together; sending clears the composer immediately. The chat toolbar combines text, push-to-talk, calls, colorful emoji and image input. Proactive messages are always silent and pause after at most one optional unanswered follow-up. Voice calls have a dedicated avatar screen, variable ringing waits and cancellation-safe outcomes. New relationships open contact gradually while ordinary text and push-to-talk remain available.

Confirmed first-run mode is saved across restarts. Fresh installations include Alpine 16 with its renderer and cloth configuration; existing avatar choices are preserved. Model 2 is retained as a fallback. The large audio-driven motion component remains Model 2-specific and is skipped for Alpine 16. Base resources are unchanged. This release does not include developer conversations, memory or credentials. Full microphone/video sessions and every supported device were not revalidated.

## 0.1.15

[原版本说明](https://github.com/ycwdjb599-hub/ai-companion-desktop/releases/tag/v0.1.15)：连续文字消息列表、保存反馈与设置页切换改进。
