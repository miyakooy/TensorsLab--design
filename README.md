---
name: TensorsLab Design
description: High-fidelity UI prototypes, marketing pages, presentation decks, infographics. 为 TensorsLab AI 产品设计。AI 产品原型/UI 设计/营销页面/演示文稿. AI 디자인/프론트엔드 プロトタイプ/マーケティングページ/プレゼンテーションシート.
title: TensorsLab Design - AI Product Design Skill for Claude Code
keywords: AI design skill, Claude Code, frontend prototype, UI design, marketing page, presentation deck, infographic, HTML design, no-code design, AI 产品设计, UI 设计,  prototyping,  プロトタイプ, AI 디자인, 프론트엔드
language: en-US
---

# TensorsLab Design

**One prompt, deliverable design.**

High-fidelity prototypes, marketing pages, presentation decks, infographics — a design skill for TensorsLab AI products.

```
npx skills add miyakooy/TensorsLab--design -y
```

Then talk to your agent:

```
"Create a PPT for AI product manager, recommend 3 styles"
"Design a TensorsLab homepage, reference Vercel"
"Make a model comparison page with metrics"
```

---

## Capabilities

| Capability | Deliverable | Time |
|------------|-----------|------|
| Interactive Prototype (App/Web)| Single HTML · Real device frame · Clickable | 10–15 min |
| Product Homepage | Landing, pricing, docs pages | 10–15 min |
| Presentation Deck | HTML deck + editable PPTX | 15–25 min |
| Infographics | PDF / PNG / SVG export | 8–12 min |
| Design Advisor | 2–3 directions + Demo | 5 min |
| 5-Dimension Review | Radar chart + Fix list | 3 min |

---

## Design Principles

### Junior Designer Workflow

Default: show assumptions first, wait for confirmation, then dive deep.

- List questions upfront before coding
- Write assumptions + placeholders in HTML
- Show content → variants → tweaks at each step
- Browser verify before delivery

### Anti-AI Slop

Avoid purple gradients, emoji icons, rounded corners + left border accent, Inter for display titles. Use CSS Grid + carefully chosen fonts and colors.

### Brand Assets

When working with specific brands:
1. Ask for brand guidelines
2. Scrape official pages for colors
3. Freeze to brand-spec.md

---

## Included Components

```
assets/
├── animations.jsx      # Motion primitives
├── ios_frame.jsx        # iPhone frame
├── android_frame.jsx   # Android frame
├── macos_window.jsx     # macOS window
├── browser_window.jsx   # Browser frame
├── deck_stage.js       # Deck presentation
└── design_canvas.jsx   # Variant comparison
```

---

## Demo Gallery

Try these demos:

- [Homepage Hero](demos/hero.html) — Modular homepage with layout switching
- [Style Board](demos/style.html) — Visual style reference
- [Model Page](demos/model.html) — Product documentation page
- [Pricing](demos/pricing.html) — Pricing tier comparison
- [Design Canvas](demos/design-canvas.html) — Variant comparison
- [Device Frames](demos/frames.html) — iOS/Android/Browser frames
- [Deck Stage](demos/deck-stage.html) — Presentation deck
- [Motion](demos/motion.html) — Animation primitives

---

## Limitations

- **No Figma-level editing**. Output is HTML — screenshot, record, or export.
- **Blank-brand designs score lower**. Brand assets improve quality.
- **3D / physics / particles out of scope**. 2D planar design only.

This is an 80-point skill. For those who don't want to open a GUI, 80 points is enough.

---

## Installation

```bash
npx skills add miyakooy/TensorsLab--design -y
```

Supported agents: Claude Code, Cursor, Codex, OpenClaw, and other skills-compatible agents.

---

## Related Skills

- [huashu-design](https://github.com/alchaincyf/huashu-design) — Similar design skill with more animation capabilities
- [Claude Design](https://claude.ai/design) — Official AI design tool

---

## License

MIT License. Personal use free. Commercial use requires permission.

---

## Changelog

- v1.0 (2026-04) — Initial release with 8 component templates
- v1.1 (2026-04) — Added pricing page, modular hero layouts
- v1.2 (2026-04) — SEO optimization, bilingual README
- v1.3 (2026-04) — Multilingual triggers in front matter
