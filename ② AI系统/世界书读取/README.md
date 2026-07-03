# 世界书读取 — 从 Obsidian 库获取知识

从用户的 Obsidian 知识库中读取世界设定、风格参考等信息的方法。

## 数据源

| 源 | 路径 | 用途 |
|----|------|------|
| 本库 | E:\Obsidian\狂澜仙欲录：玄阴\ | 项目自身内容 |
| 随笔库 | E:\Obsidian\随笔\ | 新增世界设定，标记 #狂澜仙欲录 |
| 风格库 | nsfw-style-guides（RAG） | NSFW 写作风格参考 |

## 查询方法

- RAG 查询：`python obsidian_rag.py query nsfw-style-guides <问题>`
- 向量引擎：Ollama bge-m3（维度 1024）
- 向量存储：.rag_data/（numpy + JSON）

## 约定

- 创作前先查相关设定，确保一致性
- 新设定写入随笔库并打标签
- 本库内容直接通过文件路径读取
