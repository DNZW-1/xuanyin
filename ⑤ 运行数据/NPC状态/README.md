# NPC状态 — NPC实时数据

所有 NPC 的运行时状态。与 ③ 世界数据库/角色 中的模板一一对应。

## 每个 NPC 的数据

| 字段 | 说明 |
|------|------|
| role | 身份 |
| affinity | 好感度（0-100） |
| intimacy | 亲密度（0-100） |
| status | 状态（存活/受伤/昏迷/死亡） |
| location | 当前位置 |
| relationship_stage | 关系阶段 |
| notes | 特殊备注 |

## 存储格式

推荐 JSON 对象，key 为角色名：

```json
{
  "冷凝霜": {
    "affinity": 65,
    "intimacy": 70,
    "status": "存活",
    "location": "玄阴山·主峰",
    "notes": "已推倒"
  }
}
```
