# Design Critique Guide - 5 Dimension Expert Review

> 5-dimension expert review system with radar chart visualization.
> Output: Keep / Fix / Quick Wins action list.

## 5 Dimensions

| Dimension | Score (0-10) | Description |
|-----------|:------------:|-------------|
| **Philosophy Alignment** | ___ | Design matches intended philosophy/style |
| **Visual Hierarchy** | ___ | Clear information structure and priority |
| **Detail Execution** | ___ | Pixel-perfect implementation quality |
| **Functionality** | ___ | Works as intended, interactions work |
| **Innovation** | ___ | Novel solutions and creative touches |

### Score Interpretation

- **9-10**: Exceptional, production-ready
- **7-8**: Good, minor polish needed
- **5-6**: Acceptable but needs significant work
- **3-4**: Major issues, needs redesign
- **1-2**: Critical failure, restart recommended

---

## Review Output Format

### Radar Chart Data

```javascript
{
  philosophy: 8,
  hierarchy: 7,
  detail: 9,
  functionality: 8,
  innovation: 6
}
```

### Action Items

#### ✓ Keep (Score 7+)
- List what works well and should be preserved

#### Fix (Score 4-6)  
- List issues that need revision

#### Quick Wins (Score <4 + Easy Fix)
- List critical but easy-to-fix items

---

## Review Checklist by Dimension

### 1. Philosophy Alignment (7+ to Pass)

- [ ] Style matches selected design philosophy (from design-styles.md)
- [ ] Prompt DNA correctly applied
- [ ] Color palette appropriate for style
- [ ] Typography fits style family
- [ ] Avoided anti-AI slop tropes

### 2. Visual Hierarchy (7+ to Pass)

- [ ] Primary message immediately visible
- [ ] Clear visual priority order
- [ ] Whitespace supports hierarchy
- [ ] Type scale is intentional
- [ ] Mobile/responsive hierarchy works

### 3. Detail Execution (7+ to Pass)

- [ ] Consistent spacing (grid system)
- [ ] No orphaned elements
- [ ] Hover/active states work
- [ ] Animations are smooth (60fps)
- [ ] No layout shifts on load

### 4. Functionality (7+ to Pass)

- [ ] All links work
- [ ] Forms are usable
- [ ] Keyboard navigation works
- [ ] Touch targets 44px+
- [ ] No JavaScript errors

### 5. Innovation (7+ to Pass)

- [ ] Novel solution to problem
- [ ] Creative use of medium
- [ ] Memorable visual touch
- [ ] Different from competitors
- [ ] Pushes boundaries appropriately

---

## Review Process

1. **First Pass**: Score each dimension 1-10
2. **Second Pass**: Fill checklist items
3. **Radar Chart**: Generate visualization
4. **Actions**: Categorize into Keep/Fix/Quick Wins
5. **Verdict**: Ship if all ≥5, Fix Required if any <5

### Verdict

| Result | Condition |
|-------|-----------|
| **Ship It** | All dimensions ≥7 |
| **Fix Required** | Any dimension <5 |
| **Needs Work** | Philosophy or Hierarchy <5 |

---

## Example Output

### Scores

- Philosophy: 8
- Hierarchy: 7
- Detail: 9
- Functionality: 8
- Innovation: 6

### Keep
- Typography hierarchy is excellent
- Color usage is consistent
- Responsive layout works well
- Animations are smooth

### Fix
- Hero image needs optimization (slow load)
- Some hover states missing

### Quick Wins
- Add alt text to images
- Fix contrast on disabled button

### Verdict: **Ship It** (all scores ≥7)

---

## Integration

When user asks "review this design" or "critique":
1. Load this file
2. Apply 5-dimension review
3. Output radar chart + action list
4. Give verdict with next steps
