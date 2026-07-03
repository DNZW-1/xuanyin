# Agent Skills — Agent 技能

本目录存放 opencode 可调用的 Skill、自定义工作流、自动化脚本和工具链配置。

## 目录内容说明

- 工作流定义（如：新增角色 → 创建 定义库/角色/ → 更新 运行状态/ 关联关系）
- opcode skill 配置（learned lessons、自定义 skill）
- 自动化脚本（批量处理、校验、迁移工具）
- 测试流程定义

## 当前已有

| 资产 | 位置 | 用途 |
|------|------|------|
| learned skill | ~/.config/opencode/skills/learned/ | 全局经验教训 |
| 项目 lessons | .opencode/lessons.md | 本项目特定教训 |

## 编写规则

1. Skill 文件格式遵循 opencode skill 规范
2. 工作流用清晰的步骤列表描述，每个步骤包含命令和预期结果
3. 自动化脚本注明依赖环境（Python 版本、Node.js 等）
4. 所有文件 >15 行正文
