---
name: stillpoint-post-design
description: Design system and typographic guidelines for creating StillPoint branded Instagram posts and social graphics. Use this skill whenever creating, editing, rebuilding, or critiquing any StillPoint Instagram post, social image, or HTML-based graphic. Triggers on: "make a post", "rebuild the posts", "redesign", "create an instagram image", "fix the typography", "adjust the layout", "new post design", "apply the design system". Always consult this skill before writing HTML for any StillPoint visual content.
---

# StillPoint Post Design System

A living design system for StillPoint branded Instagram posts and social graphics. Built from first principles, iterative testing, and the five core web design disciplines: typography, layout, color, visual hierarchy, and conversion thinking.

---

## Format Specification

| Property | Value |
|----------|-------|
| Canvas size | 540×675px CSS (renders to 1080×1350px at 2x) |
| Aspect ratio | 4:5 portrait (Instagram feed optimized) |
| Device scale | `device_scale_factor=2` in Playwright |
| Output | PNG via Playwright headless Chromium |

**Why 4:5?** Portrait posts take up more vertical real estate in the Instagram feed than square posts, increasing stop-scroll probability.

---

## Typography System

Typography is the single most important design element. Text takes up the most real estate. Use a deliberate type scale — never eyeball font sizes.

### Type Scale (Locked)

| Role | CSS Size | Actual px at 2x | Font | Color |
|------|----------|-----------------|------|-------|
| Headline | 38px | 76px | Georgia serif | #1a1a1a |
| Headline italic | 38px | 76px | Georgia serif italic | #2a2a2a |
| Closing / emphasis | 25px | 50px | Georgia serif italic | #2a2a2a |
| Body / detail text | 21px | 42px | Helvetica Neue, weight 300 | #555 |
| Quote lines | 38px | 76px | Georgia serif italic | #1a1a1a |
| Eyebrow / product label | 13–14px | 26–28px | Helvetica Neue, letter-spacing 0.2em, uppercase | #aaa |
| Top mark / bottom wordmark | 13px | 26px | Helvetica Neue, letter-spacing 0.2em, uppercase | #999 |
| URL (bottom right) | 13px | 26px | Helvetica Neue, letter-spacing 0.04em | #999 |

### Typography Rules (from Major Third Scale principles)

1. **Scale by ~25% between levels.** Each heading tier should be approximately 1.25× the size below it. Our 21→25→38px progression follows this.

2. **Body text line height = 1.5** (150% of font size). This gives text room to breathe.

3. **Heading line height = 1.2–1.25.** As text gets bigger, tighten line height for impact and scannability.

4. **Body letter spacing: don't touch it.** Leave at default for maximum legibility.

5. **Heading/label letter spacing: use sparingly.** Uppercase labels use 0.18–0.22em tracking. Headline Georgia text uses default tracking.

6. **Minimum body text size: 21px CSS (42px actual).** Below this, text strains on mobile. The research-backed minimum for Instagram graphics is 30pt — our 42px actual exceeds this safely.

7. **Two fonts maximum.** Georgia serif for voice/copy. Helvetica Neue for structure/labels. Never introduce a third typeface.

---

## Color System

Pro designers use color intentionally, not abundantly. Limit the palette and give each color a specific job.

### Palette (60/30/10 Rule Applied)

| Role | Hex | Usage |
|------|-----|-------|
| Primary background (60%) | #f5f2ee | Default cream — all text posts |
| Secondary background (30%) | #f0ede8 | Slightly darker cream — product posts (Post 09 style) |
| Page background | #e8e4de | Outer body color (not part of post frame) |
| Headline text | #1a1a1a | Maximum contrast, primary reading |
| Strong body / closing | #2a2a2a | Dark — for closing lines, emphasis italic |
| Body text | #555 | Secondary reading — detail bullets |
| Supporting / muted | #666–#777 | Tertiary copy, sublines |
| Labels / eyebrow | #aaa | Structural labels, product names |
| Wordmark / URL | #999 | Bottom bar elements |
| Dots / rules | #999 | Bullet dots, horizontal rules |
| Divider lines | #ddd | Hairline rules between sections |
| Quote mark accent | #ddd | Decorative opening quote marks |

### Color Rules

1. **No accent colors in the current system.** StillPoint's brand uses restraint. The cream-and-near-black palette IS the brand. Don't add blues, greens, or other colors without explicit approval.

2. **Use opacity, not new colors.** If a variation is needed, adjust opacity of an existing color.

3. **Contrast check before publishing.** Headline (#1a1a1a on #f5f2ee) passes WCAG AAA. Body (#555 on #f5f2ee) passes WCAG AA for large text. URL/wordmark (#999) is intentionally below AA — acceptable for decorative secondary elements only.

4. **Contrast thresholds (WCAG):**
   - Small text: 4.5:1 minimum (AA)
   - Large text (18px+ or 14px+ bold): 3:1 minimum (AA)
   - Our headline contrast ratio: ~12:1 ✅

---

## Layout & Spacing System

### 8-Point Grid

All spacing is a multiple of 8. This mirrors Google Material Design and Apple's design system.

| Use | Value |
|-----|-------|
| Outer padding (post frame) | 52px top/sides, 44px bottom |
| Gap between headline lines | 8px |
| Gap below headline block | 32–36px |
| Gap between bullet rows | 14px |
| Gap above closing/divider | 24px |
| Gap between sections | 24–32px |
| Bottom bar — no extra margin needed | flush to padding |

### Layout Structure (top → bottom)

```
[ Top mark: STILLPOINT™ ]           ← always present
[ Eyebrow label ]                   ← optional (product posts)
[ Headline block ]                  ← primary hook, 38px
[ Body content ]                    ← bullets, quote lines, or copy
[ Divider rule ]                    ← separates body from closing
[ Closing / emphasis line ]         ← 25px italic, dark (#2a2a2a)
[ Bottom bar: wordmark + URL ]      ← always present
```

### Visual Hierarchy Principles

People scan, they don't read. The layout must guide the eye in priority order.

1. **Proximity:** Keep related elements close. The headline and its italic subhead are visually grouped. The closing line is separated by a rule — it's its own thought.

2. **Size signals importance.** 38px headline > 25px closing > 21px body > 13px label. Never reverse this hierarchy.

3. **Contrast signals reading priority.** #1a1a1a (headline) vs #555 (body) vs #aaa (label) creates three distinct reading tiers without using color.

4. **Alignment = clarity.** All text left-aligns from a consistent left edge. The URL right-aligns in the bottom bar for balance. No centered text.

5. **White space is content.** Generous padding (52px) and vertical breathing room make the post feel calm — which mirrors the product's purpose.

---

## Post Structure Templates

### Template A: Quote Post (Posts 05, 10)
```html
[ STILLPOINT™ ]
[ Large decorative " ]
[ Quote lines — 38px italic Georgia ]
[ Attribution — 14px uppercase Helvetica Neue ]
[ — — — divider — — — ]
[ Response line — 21px italic ]
[ Closing line — 25px italic #2a2a2a ]
[ STILLPOINT™ · trystillpoint.life ]
```

### Template B: Copy/Statement Post (Posts 01, 06, 07, 08)
```html
[ STILLPOINT™ ]
[ Rule or eyebrow ]
[ Headline statement — 38px Georgia ]
[ Italic subline — 38px Georgia italic ]
[ Supporting body — 21px Helvetica Neue ]
[ — — — divider — — — ]
[ Closing emphasis — 25px italic ]
[ STILLPOINT™ · trystillpoint.life ]
```

### Template C: Product Post (Post 09)
```html
[ STILLPOINT™ ]
[ STILLPOINT AIR — eyebrow label ]
[ Headline — 38px ]
[ Headline italic — 38px ]
[ Bullet list — 21px Helvetica Neue, dot color #999 ]
[ — — — divider — — — ]
[ Closing italic — 25px #2a2a2a ]
[ STILLPOINT™ · trystillpoint.life ]
```

---

## Rendering

### Render All 10 Posts
```bash
python3 /sessions/brave-trusting-thompson/render_posts_hires.py
```

### Render Single Post
Edit `render_single.py` with the post name, then:
```bash
python3 /sessions/brave-trusting-thompson/render_single.py
```

### Render Script Settings
```python
device_scale_factor = 2       # 540px CSS → 1080px actual
viewport = 540 × 675          # CSS dimensions
selector = ".post"            # captures only the post frame, not caption box
output_format = PNG
```

---

## Quality Checklist

Before finalizing any post, verify:

- [ ] Headline ≥ 38px
- [ ] Body text ≥ 21px
- [ ] Closing line = 25px, color #2a2a2a (darker than body)
- [ ] Bottom wordmark reads **StillPoint™** (with ™ mark, consistent with top mark)
- [ ] URL `trystillpoint.life` visible, color #999 (not #bbb — too faint)
- [ ] Bullet dots color #999 (not #bbb)
- [ ] All spacing multiples of 8
- [ ] No third typeface introduced
- [ ] Caption box included in HTML with ready-to-paste text and hashtags
- [ ] File saved to `/stillpoint/instagram/post-XX-name.html`
- [ ] PNG rendered to `/stillpoint/instagram/png/post-XX-name.png` at 1080×1350

---

## Conversion Thinking

Every post has one job. Define it before writing copy.

| Post type | Job | CTA location |
|-----------|-----|-------------|
| Product post (09) | Explain what it is → drive to link in bio | URL in bottom bar |
| Quote/philosophy post | Build trust, establish voice → follow | Brand identity, no hard CTA |
| Beginner post | Normalize the practice → new audience | Soft: "StillPoint makes it easier" |
| Pre-order/launch | Reserve → conversion | Caption CTA + URL in bar |

**Trust elements to include in product posts:** "Handcrafted in the USA," "Ships May 2026," "First Batch: 400 units," "Individual experiences vary."

---

## Source References

- YouTube: *The Only 5 Web Design Skills That Matter* — typography scale, 8-point grid, 60/30/10 color rule, visual hierarchy principles, conversion thinking
- StillPoint post iterations (2026-03-16) — hands-on type scale refinement: 44px → 40px → 38px headline, 18px → 22px → 21px body
- WCAG 2.1 AA — contrast ratio standards (4.5:1 small text, 3:1 large text)
- Design critique session (2026-03-16) — identified: URL too faint (#bbb→#999), dots too faint (#bbb→#999), ™ inconsistency fixed

---

*Last updated: 2026-03-16 | Canon version: v2.2*
