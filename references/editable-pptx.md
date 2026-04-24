# Editable PPTX Export

> How to export editable PowerPoint from HTML.

## Overview

Export editable PPTX when users need to:
- Edit text in PowerPoint
- Collaborate with others using PowerPoint
- Present using native PowerPoint

## Method: html2pptx.js

### Usage

```bash
node scripts/html2pptx.js input.html output.pptx
```

### How It Works

1. Parse HTML DOM
2. Read computed styles for each element
3. Map HTML to PowerPoint shapes/text
4. Preserve text boxes (not images!)
5. Generate .pptx file

---

## What Transfers Well

| HTML Element | PPTX Equivalent |
|--------------|---------------|
| `<h1>` | Title text |
| `<h2>` | Subtitle text |
| `<p>` | Body text |
| `<div>` | Textbox / shape |
| `<img>` | Embedded image |
| Colors | Fill color |
| Font-size | Font size |
| Font-weight | Bold |

---

## What Needs Manual Fix

- Complex CSS grid layouts
- Custom fonts (converted to closest system font)
- Certain animations
- Images may lose quality
- Complex shadows/effects

---

## Best Practices for Editable Export

### Do

- Use simple layouts
- Stick to system fonts
- Keep colors simple
- Use standard PowerPoint shapes

### Don't

- Overuse custom fonts
- Complex positioned elements
- Heavy CSS effects
- Nested complex tables

---

## Workflow

1. Design in HTML using deck_stage.js
2. Test in browser
3. Run html2pptx.js export
4. Open in PowerPoint
5. Fix any layout issues
6. Done!
