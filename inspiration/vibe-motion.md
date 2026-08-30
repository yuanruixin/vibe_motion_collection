# VibeMotion 库与项目资料合集

> 整理时间：2026-08-30 ｜ 信息来源：国外官网、GitHub、技能社区、中文技术社区

## 一、VibeMotion 是什么

**Vibe-Motion** 是 "Vibe Coding"（氛围编程）理念在**动效设计**领域的延伸：用自然语言对话生成专业级动态图形（Motion Graphics）。

核心架构（由 Higgsfield AI 率先推出）：

- **Anthropic Claude** 负责理解自然语言并生成代码
- **Remotion**（基于 React 的程序化视频框架）负责确定性渲染
- 区别于 Sora/Veo 等"像素预测"式视频生成：**生成的是真实代码**，文字不会破碎、颜色精确可控、可无限迭代修改、支持 4K/60fps 输出

---

## 二、核心库与开源项目（程序员重点）

### 1. Higgsfield Vibe Motion（概念发源地）

- 网址：https://higgsfield.ai/vibe-motion
- 形式：网页聊天式平台，Claude + Remotion 驱动
- 价格：有免费额度，付费约 $9~17.4/月起
- 用途：文字动画、Logo 动画、信息图、演示文稿、社媒动效

### 2. Remotion（最重要的底层引擎，必学）

- 网址：https://remotion.dev ｜ GitHub: https://github.com/remotion-dev/remotion
- 完全开源免费的 React 视频框架，用代码写视频
- 任何 VibeMotion 工作流的地基；配合 Claude/Cursor 等任意 AI 编程工具即可自己搭一套"平替"

### 3. GurYN/vibe-motion（开源完整应用）

- GitHub: https://github.com/GurYN/vibe-motion
- 技术栈：Next.js 16 + React 19 + Remotion 4 + Claude Code CLI + Prisma + xterm.js
- 功能齐全：项目管理、资产拖拽上传、内嵌终端、内嵌 Remotion Studio、MP4/WebM/GIF 导出
- 适合想研究完整架构或自部署的开发者（需 Claude Pro/Max 订阅或 API Key）

### 4. amirmushichge/VibeMotion（本地 AI 视频编辑器）

- GitHub: https://github.com/amirmushichge/VibeMotion （pre-alpha）
- Windows 本地运行，集成了 LTX-2.3 视频模型、Gemma、Ollama、faster-whisper、FFmpeg
- 亮点：支持 **Figma 图层导入动画**、Prompt 驱动运动块、本地渲染 MP4
- 适合有 NVIDIA GPU、想全本地化跑 AI 视频管线的玩家

### 5. Higgsfield Claude Skill（higgsfield-vibe-motion）

- 仓库：https://github.com/OSideMedia/higgsfield-ai-prompt-skill
- 安装：`npx skills add OSideMedia/higgsfield-ai-prompt-skill --skill higgsfield-vibe-motion --agent claude-code`
- 内容：Vibe Motion 的提示词模式库、模板分类、调色/调速工作流，可直接装进 Claude Code
- 同类技能收录站：https://claudeskills.info 、https://skillsmp.com

### 6. 中文生态的 vibe-motion 脚手架

- `create-vibe-motion` 脚手架 + `vibe-motion/skills` 技能库（含微信聊天动效、黑胶唱片机、地球飞线动画等中国特色模板）
- 三层架构：Remotion（2D）+ Three.js（3D）渲染层 / Claude Code 代理层 / SRT 转视频等工作流层
- 参考：CSDN《vibe-motion 快速上手操作指南（Windows 优化版）》https://blog.csdn.net/HT2461110275/article/details/162732149 （集成了字节 Trae、腾讯 QClaw 等国内免费 AI Agent 方案）

---

## 三、配套动效/组件库（Vibe Coding 生态）

| 名称                           | 网址                          | 特点                                                         |
| ------------------------------ | ----------------------------- | ------------------------------------------------------------ |
| **Motion**（原 Framer Motion） | https://motion.dev            | 生产级动效引擎，弹簧物理/布局动画/手势，400+ 示例            |
| **Motion Primitives**          | https://motion-primitives.com | Framer Motion + Tailwind 的复制粘贴式动画组件，`npm install motion-primitives` |
| **React Bits**                 | https://reactbits.dev         | 165+ 免费开源动画组件（极光背景、文字显影、光效），无运行时依赖 |
| **Aceternity UI**              | https://ui.aceternity.com     | 200+ 高级感组件，"一看就贵"的官网风                          |
| **Anime.js**                   | https://animejs.com           | 轻量 JS 动画引擎，时间线/弹簧/滚动联动/SVG 变形              |
| **Uiverse**                    | https://uiverse.io            | 7400+ 社区开源 UI 元素，可导出 HTML/CSS/Tailwind/React       |
| **21st.dev**                   | https://21st.dev              | 10000+ React/Tailwind 组件注册表，shadcn registry 格式       |
| **shadcn/ui**                  | https://ui.shadcn.com         | 开放代码、AI-Ready 的组件基石                                |
| **MotionSites**                | https://motionsites.ai        | 100+ 动效网站的 AI 提示词库，短视频"10秒复刻炫酷网页"的 Prompt 源头 |
| **Design Prompts**             | https://www.designprompts.dev | 30+ 视觉风格的万字级 AI 提示词（治"AI 味"）                  |

---

## 四、灵感与参考网站

- **Awwwards** — https://www.awwwards.com （行业上限、前沿交互趋势）
- **Landbook** — https://land-book.com （按类型/风格/行业筛选的网页图库）
- **Curated Design** — https://curated.design （人工筛选，可按 Hero/Pricing 等区块找参考）
- **Landing.Gallery** — https://www.landing.gallery （1600+ 落地页，提供面向 Coding Agent 的 MCP 入口）
- **SaaS Landing Page** — https://saaslandingpage.com （约 950 个 SaaS 官网案例）
- **Mobbin** — https://mobbin.com （62 万+ 真实 App/Web 界面截图）
- **Craftwork** — https://craftwork.design/curated/websites
- **Navbar Gallery / CTA Gallery / Rebrand Gallery** — 导航栏、按钮、品牌重塑专项灵感库

---

## 五、社区与学习资料

**国外社区：**

- GitHub — 搜 `vibe-motion`、`remotion`、`motion-primitives` 等关键词；各项目均接受 PR 贡献
- Remotion 官方 Discord — Remotion 框架的一手讨论区
- X/Twitter — 关注 Higgsfield AI、@Ibelick（Motion Primitives 作者）、Remotion 团队
- Reddit — r/webdev、r/reactjs、r/remotion
- https://vibecoder.me — 专门面向 Vibe Coder 的工具评测站（含 Motion Primitives 专文）
- https://vibemotion.net — Vibe-Motion 概念科普站（含 10 个 Prompt 模板）
- https://www.pinterest.com/ - 图片社区，寻找你的灵感吧
**中文社区：**

- CSDN / 掘金 — 搜"vibe-motion 快速上手""Remotion 教程"，已有 Windows 优化版实践指南
- 素材集市 https://www.sucaijishi.com — 《玩 VibeCoding 必备的 5 个宝藏网站》等转载文章
- 公众号 / 知乎 — 搜"Vibe Coding 动效组件""AI 审美"有大量同主题清单文

**小红书 / 抖音（国内短视频平台）：**
这两类平台上相关内容主要以"宝藏网站推荐""10 秒做出炫酷网页"的形式传播，无法直接给出链接，建议用以下关键词搜索：

- 小红书：`Vibe Coding`、`vibe coding 动效`、`AI 做视频`、`Remotion`、`Cursor 网页`、`AI 审美`、`动效组件`
- 抖音：`Vibe Coding`、`AI 编程`、`炫酷网页`、`Claude 做视频`、`AI 动效`
- 这些平台上流传的网站清单（如"拯救你 AI 审美的 5 个宝藏网站"），其内容源头基本就是上表中的 MotionSites、React Bits、Uiverse、Anime.js、Aceternity UI 这几家的组合
  
---

## 六、推荐上手路线

1. **零基础快速体验**：Higgsfield Vibe Motion（免费额度）→ 聊天式生成动效
2. **程序员路线**：Remotion 官方教程 + Claude/Cursor/Trae，参考 GurYN/vibe-motion 架构
3. **提示词弹药库**：装 higgsfield-vibe-motion Skill，或抄 MotionSites / Design Prompts 的 Prompt
4. **网页动效（而非视频）**：React Bits / Motion Primitives / Motion + 21st.dev 组件，喂给 AI 改造