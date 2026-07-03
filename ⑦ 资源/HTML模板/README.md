# HTML模板 — 可复用的页面片段

可用于组装游戏页面的 HTML 片段模板。

## 规划

| 模板 | 说明 |
|------|------|
| dialogue-box.html | 对话框结构模板 |
| map-view.html | 地图容器模板 |
| inventory-grid.html | 背包网格模板 |
| save-slot.html | 存档槽位模板 |
| modal.html | 通用弹窗模板 |

## 使用方式

各模板作为独立的 .html 片段文件，通过 JavaScript 的 innerHTML 或 fetch 加载后插入 DOM。

## 约定

- 模板不含内联样式，样式在 ① 客户端/CSS/ 中
- 模板用 `{{变量名}}` 标注可替换内容
- 每个模板文件 >15 行

## 现状

当前所有 UI 是内联在 index.html 中的，尚未拆分为模板。
