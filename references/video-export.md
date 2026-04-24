# Video Export Guide

> How to export videos from HTML animations.

## Export Options

### 1. Screen Recording (Easiest)

**macOS**: Cmd+Shift+5 → Select area → Record

**Windows**: Win+G → Record

- Quick and easy
- No setup required
- Best for quick demos

### 2. HTML → MP4 via Puppeteer

```javascript
const puppeteer = require('puppeteer');
// Use animations.jsx Stage component
// Capture frame by frame or use video recording
```

### 3. html2video Scripts

Use provided scripts:
```bash
node scripts/render-video.js input.html output.mp4
```

---

## Animation Guidelines for Video Export

### Frame Rate

- **Standard**: 30fps
- **High Quality**: 60fps
- **Cinematic**: 24fps

### Duration

Keep videos short:
- **Social**: 15-30 seconds
- **Demo**: 30-60 seconds
- **Full**: 2-3 minutes max

### File Size

Target:
- **<5MB**: For web/gift
- **<25MB**: Standard sharing
- **>25MB**: Compress or host externally

---

## Optimization Tips

### Before Export

1. Remove unnecessary elements
2. Simplify animations
3. Use solid backgrounds
4. Limit color palette

### After Export

1. Compress: `ffmpeg -i input.mp4 -vcodec libx264 -crf 23 output.mp4`
2. Or use Handbrake for GUI compression

---

## Output Formats

| Format | Use For |
|--------|--------|
| MP4 | Universal, social media |
| GIF | Quick demos, (up to 10s) |
| WebM | Web, smaller size |
