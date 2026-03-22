# 建议命令
- 构建：`make build` 或 `go build ./...`
- 全量测试：`go test ./...`
- 指定包测试：`go test ./core/ -v`
- 指定测试：`go test ./core/ -run TestHandlePendingPermission -v`
- 竞态测试：`go test -race ./...`
- 选择性编译：`make build AGENTS=claudecode,codex PLATFORMS_INCLUDE=telegram` 或 `go build -tags 'no_discord no_dingtalk ...' ./cmd/cc-connect`
- 运行入口：`./cc-connect`
- 配置初始化：`mkdir -p ~/.cc-connect && cp config.example.toml ~/.cc-connect/config.toml`
- macOS 常用命令环境：zsh，路径含空格需加双引号。