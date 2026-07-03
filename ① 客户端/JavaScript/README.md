# JavaScript — 游戏引擎核心

所有 .js 文件。控制场景渲染、用户交互、存档逻辑。

## 规划

| 文件 | 说明 |
|------|------|
| engine.js | 主循环、场景管理器 |
| renderer.js | 舞台渲染、立绘更新 |
| dialogue.js | 对话系统、文字特效 |
| input.js | 键盘/鼠标事件处理 |
| save.js | 存档/读档逻辑 |
| map.js | 地图渲染和导航 |
| inventory.js | 背包系统 |

## 约定

- 使用 ES6+ 语法
- 全局命名空间 `window.XY`（玄阴缩写）
- 场景数据从外部 JSON 或数据模块加载
