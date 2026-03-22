# 完成任务后检查项
1. `go build ./...`
2. `go test ./...`
3. 如修改 core 交互逻辑，补跑相关定向测试（如 `go test ./core/ -run TestHandlePendingPermission -v`）
4. 检查是否在 core 中引入了硬编码平台/agent 名称
5. 检查所有新增用户可见文案是否已补齐 i18n
6. 清理未使用导入、调试日志与临时代码