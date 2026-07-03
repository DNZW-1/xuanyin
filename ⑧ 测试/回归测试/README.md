# 回归测试 — 每次改动的验证

每次项目变更后自动执行的验证流程。确保新改动不破坏已有功能。

## 检查清单

每次提交前手动执行：

- [ ] `git status` 确认文件改动符合预期
- [ ] 打开 ① 客户端/HTML/index.html，场景推进正常
- [ ] 检查 [[wikilinks]] 在 Obsidian 中正确跳转
- [ ] 检查 save.json 格式正确，无损坏
- [ ] 检查新文件 >15 行正文，无 stub
- [ ] 检查目录结构与 .opencode/instructions 一致
- [ ] 检查敏感信息（token/密码）未被提交

## 自动化规划

后续可编写 PowerShell 脚本实现自动检查：
- 文件行数检查
- wikilink 有效性检查
- JSON 格式校验
- 目录结构一致性检查
