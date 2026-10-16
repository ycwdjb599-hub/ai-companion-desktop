# 数据与隐私 / Data and privacy

- 聊天记录、记忆和人物实例默认保存在本机用户资料目录，不附在安装包或本仓库里。
- 调用聊天或配音 API 时，程序会发送提供该服务所必需的文本及相关上下文。服务提供方按其条款处理和计费；“本地保存”不代表云端 API 无法收到输入。
- API Key 和业务空间信息按当前 Windows 用户加密保存，不能直接复制给另一位 Windows 用户使用。
- 资源下载不需要你的聊天 API Key。程序和模型资源各自更新，私人聊天不参与发布构建。
- 连续语音需你主动开启，跟随 Windows 默认输入设备。可以关闭录音或用停止按钮取消；没有后台定期截图功能。
- 不把 Key、空间专属地址、私人对话或资料库提交到公开 Issues。上传截图前请涂掉个人信息。

Chat history, memory and character instances are stored locally and are not included in this repository or installer. API calls send the text and context needed by your chosen provider; local storage does not mean cloud providers receive no input. Keys are encrypted for the current Windows user. Public resource downloads do not receive your chat API credentials.

Continuous listening is opt-in and uses the Windows default input device. No periodic background screen capture is provided. Do not submit keys, private conversations or databases to public issues.

- 主动消息需要开启对应设置，始终静音，但生成内容仍可能产生所选服务的 API 费用。未回复时会暂停后续分享。
- 发送图片会把选中的图片提交给已配置的视觉服务；不自动读取或定期截图桌面。
- 通话是否可接与关系相关状态保存在本地；拒接不影响普通文字与按住说话。

Proactive messages are opt-in and always silent, but generation can incur API charges. Selected images are sent to the configured vision provider. Relationship/contact state stays local; ordinary text and push-to-talk remain available.
