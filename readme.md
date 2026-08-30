# 生成艺术 · 诗意动画

以 [p5.js](https://p5js.org/) 为核心的诗意动画 / 生成艺术项目。每个作品都是**单文件 HTML**，直接双击或通过本地静态服务打开即可运行，无构建、无框架。

## 作品列表

| 编号 | 名称 | 关键词 |
|---|---|---|
| 01 | 飞鸟集 · 流光（Stray Birds） | 泰戈尔《飞鸟集》选段 |
| 02 | 天青色等烟雨 · 江南彩墨 | 江南烟雨 · 彩墨 |
| 03 | 蒲公英的约定 · 视觉诗 | 蒲公英 · 视觉诗 |
| 04 | 环形诗句 · 蒲公英的约定（Dandelion Orbit） | 环形诗句 |
| 05 | 彩色的时间长河花海 · 月上泪湖-花海（Tear Lake） | 泪湖沉钟 · 时间长河 |。


## 技术栈

- **p5.js 1.11.3**（CDN 引入）
- **字体**：Google Fonts `Noto Serif SC`（中文衬线）+ `Cormorant Garamond` italic（英文）
- **画布**：9:16 竖版布局，全屏自适应，深色底基准 `#0a0e21`
- **单文件、无构建**：不引入 npm / bundler / 前端框架

## 目录结构

```
animation/
├── inspiration/              # 灵感与设计参考（只读素材）
│   └── animation-inspiration.html
├── motion/                   # 动画作品，每个作品一个编号目录
└── README.md
```

## 贡献 / 制作约定

新作按序号递增命名 `NN-name/`，每个作品目录需包含 `index.html`。改动画前先改对应 `prompt.md` 参数表，再同步实现。详细约定见 [AGENTS.md](AGENTS.md)。
