# Prompt: Framer Single-Page Landing Build — Still Point (v1)

## Purpose
Generate a Framer-ready, claims-safe, conversion-focused single-page landing plan and the exact copy needed to implement it.

This prompt is used to:
- Produce the v1 page structure from canon
- Write final copy blocks (not just suggestions)
- Ensure “what it is / what it is not” clarity in <10 seconds
- Predict conversion friction and remove it via layout + copy

---

## Canon References (source of truth)
Use these as authoritative context:
- ../canon/site-brief.md
- ../canon/site-map-and-copy.md
- ../canon/product-canon.md
- ../canon/claims-guardrails.md
- ../canon/mission-identity.md
- ../canon/archetype-profiles.md

Do not invent product capabilities or claims beyond canon.

---

## Input
Provide any of the following (optional; if missing, choose conservative defaults and label them clearly):
- Primary emphasis: meditation-first or sleep-first
- CTA text preference: “Join the waitlist” or “Get early access”
- Hero option preference (A/B/C from `site-brief.md`) or write a new canon-consistent hero
- Any brand constraints for visuals (background, color, photography style)
- Any existing draft copy you want rewritten

---

## Output (must follow this structure)

### 1) One-screen clarity module (top of page)
Provide:
- Headline
- Subhead (max ~2 sentences)
- 3 fast-scan bullets that MUST include:
  - external-only / never enters nostrils
  - airflow unobstructed
  - amplifies breath sensation to help attention return
- Primary CTA button text + microcopy beneath (optional)
- Above-the-fold visual spec (exact shot suggestions)

### 2) Full page section outline (in order)
For each section:
- Section name
- Goal (1 sentence)
- Layout notes (desktop + mobile)
- Exact copy (headlines, body, bullets, CTA if applicable)
- Visual requirements (specific shots/graphics)

### 3) “What it is / What it is not” clarity block
Write the block exactly as it should appear on the page, optimized for skim reading.

### 4) Mechanism explanation (simple, grounded)
Write a short mechanism section that stays inside canon:
- 3-step flow: “breath more vivid → attention returns → practice steadies”
- Include the fit truth: anchors on sidewalls; floats around tip; airflow unobstructed

### 5) Use cases module (claims-safe)
Write a compact grid/list covering canon use cases:
- Meditation
- Settling between tasks
- Sleep support (safe phrasing)
- Travel/public use

### 6) FAQ (short answers)
Include at minimum:
- Does it block breathing?
- Does it go inside the nostrils?
- Is it a nasal dilator?
- Can I talk while wearing it?
- How do I clean it?
- How long do I wear it?
- What size / will it fit?
- Is it comfortable for bedtime?

### 7) Trust & proof placeholders
Provide:
- Founder story micro-block (2–4 sentences, claims-safe)
- Suggested proof slots (testimonials/practitioner quotes) with placeholder text rules

### 8) Final CTA section
Write the final CTA section copy (headline, subhead, button, reassurance).

### 9) Framer implementation checklist
Give a practical checklist:
- Sections as Frames
- Component list (buttons, FAQ accordion, testimonial card, image blocks)
- Responsive breakpoints + typography guidance
- Accessibility basics (contrast, focus states, heading order)

### 10) SEO pack (ready to paste)
Provide:
- Page title (<= 60 chars)
- Meta description (<= 155 chars)
- OG title + OG description
- 5 image alt text lines (generic but specific enough)

---

## Claims Safety Verification (required)
At the end, include:
- Any phrases that risk drifting into medical claims (if any)
- Safer rewrites for each flagged phrase

