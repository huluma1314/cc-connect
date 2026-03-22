# 风格与约定
- core/ 必须保持平台与 agent 无关，禁止在 core 中硬编码平台/agent 名称；优先使用 optional capability interface。
- 错误处理统一使用 fmt.Errorf 包装上下文，运行期日志统一使用 slog。
- 并发场景使用 context、mutex、atomic、sync.Once 等保证安全。
- 所有面向用户的文案必须进入 core/i18n.go，并补齐 EN/ZH/ZH-TW/JA/ES。
- 遵循标准 Go 约定：gofmt、go vet、函数保持聚焦，命名避免重复赘述。
- 仅允许 init() 用于 agent/platform 注册。