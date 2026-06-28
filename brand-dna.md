# Brand DNA — 你的品牌基因

> ⚠️ **使用前必须完成此文件的配置。** 把下面所有 `YOUR_XXX` 占位符替换成你自己的品牌信息。

---

## 🎨 品牌三色

| 色名 | 色值 | 用途 |
|------|------|------|
| 主色 | `YOUR_PRIMARY_COLOR` | 主色调、标题、超链接、重点标记 |
| 强调色 | `YOUR_ACCENT_COLOR` | 强调、装饰、badges、高亮 |
| 点缀色 | `YOUR_HIGHLIGHT_COLOR` | 点缀、CTA、标签（用量最少） |

三色比例原则：主色60% · 强调色30% · 点缀色10%

---

## 👤 头像/IP形象

请将你的头像文件放入 `assets/avatar.jpg`（建议正方形，至少 400×400px）。

如果你有完整IP形象（全身/半身），放入 `assets/character.png`。

### 使用规则
- 需要头像时优先用 `assets/avatar.jpg`
- 是否在页面中使用IP形象由你决定，不强制

---

## 🔤 字体基因

### 核心原则
- **标题用衬线，正文用无衬线** — 混搭产生节奏
- **中英文搭配** — 英文做装饰/标签，中文承载内容
- **字号对比极端** — 大的要很大，小的要真的小

### 推荐字体池

| 场景 | 推荐 | 备注 |
|------|------|------|
| 英文装饰/标题 | `Fraunces` (italic) | 有品质的衬线体 |
| 英文手写/轻松 | `Caveat` | 手绘感、标注、注释 |
| 英文等宽/终端 | `Fira Code` | 技术/终端场景专用 |
| 中文标题 | `Noto Serif SC` (900) | 衬线体，品质感 |
| 中文正文 | `Noto Sans SC` + 系统栈 | 跨平台无衬线 |

> 💡 如果你有自己偏好的字体，直接替换上面的推荐即可。

### 字号系统（fluid sizing）
- Hero大标题: `clamp(2.8rem, 7vw, 5.5rem)`
- Section标题: `clamp(1.6rem, 4vw, 2.6rem)`
- 卡片标题: `1.15rem ~ 1.4rem`
- 正文: `16px`
- 辅助文字: `0.78rem ~ 0.85rem`
- 大装饰数字: `clamp(3rem, 8vw, 7rem)` + `opacity: 0.12~0.2`

---

## ✨ 气质关键词

设计出来的东西应该让人觉得：

- **可爱但有品质** — 不是幼儿风也不是奢侈风
- **手绘蜡笔感** — 有温度、有人味
- **不像AI** — 这是最高优先级的约束
- **有设计师眼光** — 细节讲究、间距精确、色彩克制
- **温暖但不幼稚** — 有内容有深度

> 💡 请根据你自己的品牌调性修改上面的关键词。

---

## 🎨 配色扩展原则

当三色不够用时：

- 背景偏暖：`#fefcf6`（主背景）、`#faf6eb`（深奶）— 或替换为你自己的背景色
- 文字非纯黑：用 `#1A1A2E`（墨色）或 `#1a1a1a`
- 次要文字：`#4A4A5A`、`#555`、`#888`
- 绝不用纯黑 `#000` 或纯白 `#fff`
- 暗色场景底色：`#151821`、`#0d1117`
- 径向渐变制造层次，不用纯平色

---

## 🚫 通用禁忌清单

| 类型 | 禁止 |
|------|------|
| 配色 | 蓝紫渐变、cyan、neon、纯黑白、AI常用的冷灰蓝调 |
| 字体 | Inter/Roboto/Arial等overused字体 |
| 布局 | 所有section居中、千篇一律卡片网格、cards嵌套cards |
| 动效 | bounce/elastic、animate width/height、无限循环动画 |
| 装饰 | glassmorphism、圆角矩形+阴影千篇一律、渐变文字、AI光效 |
| 整体 | 看起来像AI生成的通用模板 |
| 图片 | AI生成的stock photo风、过度滤镜、无意义装饰图 |
| 默认样式 | HTML默认blockquote/ul/ol/table——所有组件必须从components.md选用 |

### 自检问题
做完设计后问自己：
1. 这个页面截图发到社交媒体，会不会被人评论"又是AI做的"？
2. 能不能一眼认出这是你的品牌？
3. 有没有哪个部分让你觉得"见过很多次了"？

---

## 📐 通用间距原则

- Section之间: `clamp(80px, 12vh, 160px)`
- 内容块之间: `clamp(40px, 6vw, 100px)`
- 卡片内padding: `clamp(28px, 3vw, 44px)`
- 元素间gap: `clamp(24px, 3vw, 48px)`
- 全部用 `clamp()` 做fluid sizing
- `max-width: 1300px` + `margin: 0 auto` 约束内容宽度

---

## 📱 响应式通用规则

- 断点: 900px（两栏→单栏）、600px（字号微缩）
- 移动端是"重新排列"不是"缩小"
- 尊重 `prefers-reduced-motion`
- 移动端不隐藏内容——adapt不amputate

---

## 🔍 细节规范

- **选中文本高亮**: `::selection { background: YOUR_ACCENT_COLOR; color: #1a1a1a; }`
- **链接悬停**: 用强调色底色块或下划线，不用变色

---

*This is the foundation. Every scene file builds on top of this.*
