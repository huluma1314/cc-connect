# 项目概览
- 项目：cc-connect-pr（Go 项目）
- 目的：将本地 AI coding agent（Claude Code、Codex 等）桥接到 Telegram、Feishu、Slack 等聊天平台，实现远程会话控制。
- 关键架构：cmd/ 为入口；config/ 负责 TOML 配置；core/ 为中枢，定义 Platform/Agent/AgentSession/Engine 等接口；agent/* 与 platform/* 通过注册表插件化接入；daemon/ 负责服务化。
- 当前用户工作重点：让 Telegram 端尽量接近桌面端 Claude Code/Codex 交互体验，特别是流式输出、权限请求与 AskUserQuestion。
- 开发平台：macOS (Darwin)。