# Runtime — 运行状态

本目录存放游戏进行中的「当前状态」。这些文件会随着游戏推进不断变化，是存档系统的重要组成部分。

## 目录说明

| 目录 | 内容 | 说明 |
|------|------|------|
| Current Session/ | 当前会话：正在进行的章节、时间线、AI 上下文摘要 | 每次对话开始时读取，结束时更新 |
| Player/ | 玩家状态：苏尘的属性、境界、背包、位置、Buff、任务 | 实时变化的核心数据 |
| NPC States/ | NPC 状态：每个 NPC 当前的好感、位置、生死、特殊状态 | 与 Definitions/Characters 对应 |
| World States/ | 世界状态：天气、国家局势、事件进度、宗门关系 | 宏观状态，每小时/每天更新 |
| Inventories/ | 库存数据：商店、仓库、容器内的实例化物品 | 物品实例而非模板 |

## 数据流

1. 启动 → 读 `World States/save.json` 重建 Runtime 状态
2. 运行时 → Runtime 各目录实时更新
3. 存盘 → 汇总 Runtime 到 `World States/save.json`

## 编写规则

1. 推荐 JSON 格式（机器可读写），也可用 YAML
2. 每次状态变更必须记录到对应文件，不依赖 AI 上下文记忆
3. Runtime 文件不包含长叙事文本——叙事在 Definitions/Events 中
4. 存档即唯一真相源
