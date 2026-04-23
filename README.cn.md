---
title: TensorsLab Design - AI 产品设计 Skill (Claude Code)
description: 高保真 UI 原型、营销页面、演示 Deck、信息图表 - 为 TensorsLab AI 产品设计的 skill。一句话 prompt 交付可用设计。
keywords: AI 设计 skill, Claude Code, 前端原型, UI 设计, 营销页面, 演示文稿, 信息图表, HTML 设计, 无代码设计
language: zh-CN
---

# TensorsLab Design

**一句话 prompt，拿回一份能交付的设计。**

高保真原型、营销页面、演示 Deck、信息图表——为 TensorsLab 产品设计一枚 skill。

```
npx skills add miyakooy/TensorsLab--design -y
```

然后在 agent 里说话：

```
「做一份 AI 产品经理的演讲 PPT，推荐 3 个风格方向」
「帮我设计 TensorsLab 主页，参考 vercel 的风格」
「做一个模型对比页，展示性能指标」
```

---

## 能力表

| 能力 | 交付物 | 耗时 |
|------|--------|------|
| 交互原型（App/Web）| 单文件 HTML · 真设备框 · 可点击 | 10–15 分钟 |
| 产品主页 / 营销页 | 品牌化着陆页、定价页、文档页 | 10–15 分钟 |
| 演讲幻灯片 | HTML deck + 可编辑 PPTX | 15–25 分钟 |
| 信息图表 | 可导 PDF / PNG / SVG | 8–12 分钟 |
| 设计方向顾问 | 2–3 个方向 + Demo | 5 分钟 |
| 5 维度评审 | 雷达图 + 修复清单 | 3 分钟 |

---

## 设计原则

### Junior Designer 工作流

先 show 假设，等确认，再深入。

- 开工前列问题清单
- HTML 里写 assumptions + placeholders
- 内容 → 变体 → 微调，每步都 show
- 交付前浏览器验证

### 反 AI slop

避免紫渐变、emoji 图标、圆角+左 border accent。用 CSS Grid + 精心选择的字体。

### 品牌资产

涉及具体品牌时：
1. 问有没有 brand guidelines
2. 搜官方页抓色值
3. 固化到 brand-spec.md

---

## 包含组件

```
assets/
├── animations.jsx      # 动效原语
├── ios_frame.jsx        # iPhone 框
├── android_frame.jsx   # Android 框
├── macos_window.jsx     # macOS 窗口
├── browser_window.jsx   # 浏览器框
├── deck_stage.js       # Deck 演示
└── design_canvas.jsx   # 变体对比
```

---

## Demo 画廊

试试这些 Demo：

- [Homepage Hero](demos/hero.html) — 模块化首页
- [Style Board](demos/style.html) — 视觉风格参考
- [Model Page](demos/model.html) — 产品文档页
- [Pricing](demos/pricing.html) — 定价页
- [Design Canvas](demos/design-canvas.html) — 变体对比
- [Device Frames](demos/frames.html) — 设备框架
- [Deck Stage](demos/deck-stage.html) — 演示文稿
- [Motion](demos/motion.html) — 动效原语

---

## 限制

- **不支持 Figma 级编辑**。产出 HTML 可截图、录屏、导图。
- **空白品牌设计会掉分**。给品牌资产会更好。
- **3D / 物理 / 粒子超出边界**。只做 2D 平面设计。

这是一枚 80 分的 skill。不愿意开图形界面的人够用了。

---

## 安装

```bash
npx skills add miyakooy/TensorsLab--design -y
```

支持 agents: Claude Code, Cursor, Codex, OpenClaw 等。

---

## 更新日志

- v1.0 (2026-04) — 初始版本，8 个组件模板
- v1.1 (2026-04) — 添加定价页、模块化首页
- v1.2 (2026-04) — SEO 优化、双语 README
