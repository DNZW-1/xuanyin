# Agent技能 — Skill 和工作流

Opencode 的自定义 Skill、工作流脚本、自动化工具。

## 当前已有

| 资产 | 位置 | 用途 |
|------|------|------|
| learned skill | ~/.config/opencode/skills/learned/ | 全局经验教训 |
| 项目 lessons | .opencode/lessons.md | 本项目特定教训 |

## 规划

| 技能/工作流 | 说明 |
|-------------|------|
| 新增角色.md | 创建角色定义 → 更新 NPC 关联 |
| 新增场景.md | 创建事件定义 → 更新剧情节点 |
| 存档迁移.md | 项目重构时迁移存档数据 |
| 批量校验.md | 检查所有文件是否有 stub 和坏链 |

## 编写规则

1. 遵循 opencode skill 规范
2. 工作流用步骤列表描述，含命令和预期结果
3. 自动化脚本注明依赖环境
