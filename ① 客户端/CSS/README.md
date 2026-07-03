# CSS — 样式和主题

所有样式文件。当前样式内嵌在 HTML 中，后续将拆分至此。

## 规划

| 文件 | 说明 |
|------|------|
| main.css | 全局样式、布局、排版 |
| theme.css | 颜色主题、变量、暗色模式 |
| sprites.css | 立绘和角色动画 |
| ui.css | UI 组件样式（按钮、弹窗、进度条） |
| dialogue.css | 对话框专用样式 |

## 约定

- 使用 CSS 变量控制主题色
- 移动端适配优先
- 动画使用 transition 和 keyframes
