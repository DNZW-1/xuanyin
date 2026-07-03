# 当前章节 — 章节进度

当前正在进行的章节信息和进度状态。

## 数据字段

| 字段 | 说明 |
|------|------|
| chapter_id | 章节编号 |
| chapter_title | 章节名 |
| act | 幕/部分 |
| progress | 进度（百分比或已完成事件数/总数） |
| start_time | 章节开始时间（游戏内） |
| current_scene | 当前所在场景 |

## 存储格式

```json
{
  "chapter_id": "ch01",
  "chapter_title": "玄阴山夜袭",
  "act": 1,
  "progress": "3/7",
  "completed_scenes": ["开场", "寝殿", "双修"],
  "current_scene": "寝殿·事后"
}
```
