# 当前背包 — 持有的物品实例

玩家当前持有的所有物品实例。与 ③ 世界数据库/物品 中的模板对应。

## 数据字段

每个物品实例：

| 字段 | 说明 |
|------|------|
| item_id | 物品模板名（对应 ③ 世界数据库/物品 中的文件名） |
| quantity | 数量 |
| equipped | 是否装备 |
| durability | 耐久度（如有） |
| notes | 特殊备注 |

## 示例

```json
[
  { "item_id": "筑基丹", "quantity": 2, "equipped": false },
  { "item_id": "玄阴剑", "quantity": 1, "equipped": true },
  { "item_id": "灵石", "quantity": 500, "equipped": false }
]
```

## 数据流

- 获得物品 → 更新当前背包 → 同步到 save.json
- 使用物品 → 扣除数量 → 触发效果 → 更新玩家状态
