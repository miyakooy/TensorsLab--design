# Slide Decks - Design Guide

> How to design and build presentation decks in HTML.

## Deck Structure

### Basic Template

```html
<deck-stage>
  <section data-screen-label="01 Title">...</section>
  <section data-screen-label="02 Agenda">...</section>
  <section data-screen-label="03 Content">...</section>
  <section data-screen-label="04 Summary">...</section>
</deck-stage>
```

### Required Components

1. **Deck shell**: Use `deck_stage.js` starter
2. **Slide sections**: Each `<section>` is one slide
3. **Screen labels**: Add `data-screen-label` for reference
4. **Scaling**: Auto-scale to viewport

---

## Layout Patterns

### Title Slide
- Center alignment
- Large typography
- Minimal content
- Brand accent as background if needed

### Section Divider
- Full-bleed background color/image
- Centered section title
- High contrast

### Content Slide
- 2/3 width for content area
- Clear hierarchy: title > subtitle > body
- Consistent margins (8pt grid)

### Data/Chart Slide
- Large number or chart as visual anchor
- Supporting text in smaller type
- Source attribution below

### Closing Slide
- Minimal
- Contact or CTA
- Thank you message

---

## Typography Scale

| Element | Size (1920×1080) | Font |
|---------|----------------|------|
| Main Title | 72-96px | Bold |
| Section Title | 48-64px | Semibold |
| Subtitle | 32-36px | Medium |
| Body | 24-28px | Regular |
| Caption | 18-20px | Regular |

---

## Color Usage

### Slides

- Background: white or very light (#fafafa)
- Primary text: dark (#1a1a1a)
- Accent: Use brand color sparingly (10-15% max)
- Secondary: gray (#6b7280)

### Consistency Rules

- Max 3 colors per deck (background, text, accent)
- Use accent only for emphasis
- Keep footer/caption neutral

---

## Animation Guidelines

### Entrance Animations

- **Fade**: Subtle, 300-500ms
- **Slide up**: For title to content flow
- **None for title slide**: Keep it still

### Transitions

- Keep simple
- Avoid direction changes mid-deck
- Use same timing throughout

---

## Speaker Notes

### Adding Notes

```html
<script type="application/json" id="speaker-notes">
[
  "Welcome everyone to the presentation",
  "Today we'll cover three main topics",
  "This chart shows our key growth metric"
]
</script>
```

### Best Practices

- Write conversational scripts
- Don't repeat slide content
- Include timing cues if needed
- Focus on what to emphasize verbally

---

## Export Options

### HTML (Default)

- Self-contained HTML file
- Works in any browser
- Includes all fonts/resources

### Print to PDF

- Cmd+P / Ctrl+P
- One slide per page
- Works automatically with deck_stage.js

### PPTX (Editable)

- Use html2pptx.js script
- Exports real text boxes (not images)
- Some formatting may need manual fix

---

## Best Practices Checklist

- [ ] Use deck_stage.js (don't hand-roll)
- [ ] Keep slides 1920×1080 or 16:9 ratio
- [ ] Minimum 24px body text
- [ ] Consistent margins throughout
- [ ] Test keyboard navigation
- [ ] Add speaker notes if needed
- [ ] Verify print-to-PDF works
- [ ] Use max 6 words per bullet
- [ ] Max 6 bullets per slide
- [ ] One idea per slide
