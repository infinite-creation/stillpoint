# StillPoint Session Notes — 2026-04-02

**Session type:** SEO + Google Search Console setup + Framer site cleanup
**Canon version at end of session:** claims-guardrails.md v2.1 (updated today) / all other canon unchanged at v2.2
**GitHub status:** NOT committed — claims-guardrails.md v2.1 and SEO audit are new uncommitted files; Instagram files remain uncommitted since 2026-03-16

---

## Session Overview

A full, high-output day. Primary focus was getting trystillpoint.life properly indexed on Google and cleaning up remaining template content on the Framer site. A full SEO audit was written and saved. Google Search Console was set up from scratch, the site was verified, the sitemap was submitted, and the homepage is now confirmed indexed. Claims guardrails were updated to allow "stress relief" as a green-light term. The support page was fully de-templated via Framer MCP — contact info, intro text, and all FAQ accordions updated to StillPoint content. The payment-methods page (a template leftover) was moved to draft.

Note: An earlier automated session notes run (before the work session began) wrote an incomplete file stating "no substantive work today." This file supersedes that entry and reflects the full day's work.

---

## Work Completed This Session

### 1. SEO Audit — Full Site Analysis

A comprehensive SEO audit was written and saved to the research folder.

**Key finding at time of audit:** Google had indexed zero pages from trystillpoint.life. The site existed but was invisible to search — no Google Search Console setup, no sitemap submission.

**Audit contents:**
- Current indexation status
- Title tag and meta description review
- Keyword gap analysis (breath anchor, external meditation tool, nose-worn breath anchor)
- Technical SEO checklist (noindex flag, sitemap, robots.txt)
- Competitor context
- Content gap analysis (blog post opportunities)
- Recommended priority actions

**File saved:** `/stillpoint/research/seo-audit-2026-04-02.md` (new file)

---

### 2. Claims Guardrails Updated to v2.1 — "Stress Relief" Now Green-Light

Michael's homepage meta description contained "anxiety relief." The existing guardrails flagged this as yellow-light (use with care — anxiety is a diagnosable medical condition).

**Decision:** Swapped to "stress relief," which is meaningfully safer — stress is not a clinical diagnosis, and "stress relief" is ubiquitous in wellness marketing with much less FTC/FDA surface area.

**Guardrails changes (v2.1):**
- "stress relief" moved from yellow-light to **green-light** — approved for marketing copy and meta descriptions
- Reasoning documented in file
- "anxiety relief" remains yellow-light

**File modified:** `/stillpoint/claims-guardrails.md` → v2.1

---

### 3. Homepage Meta Description Updated — "Stress Relief" Live

Michael updated the Framer homepage meta description and published the change.

**Approved final meta description:**
> StillPoint is a handcrafted, nose-worn breath anchor that makes the breath easier to feel — supporting meditation, stress relief, and sleep. First Batch available now.

Change from previous: "anxiety relief" → "stress relief"

**Status:** Published live on trystillpoint.life ✅

---

### 4. Google Search Console Setup — Site Indexed and Sitemap Submitted

Full GSC setup completed from scratch. Michael performed the steps; Claude guided each one.

**Steps completed:**
- Property added for `trystillpoint.life` (URL prefix)
- Verified via domain name provider ✅
- URL Inspection confirmed: **"URL is on Google" / "Page is indexed"** ✅
- Sitemap submitted: `https://trystillpoint.life/sitemap.xml`
  - Status: Success ✅
  - Pages discovered: **7** ✅
- Screenshots reviewed — all four steps confirmed clean

**On robots.txt:** Search Console showed no robots.txt file. Absence is not harmful (Google defaults to "crawl everything"), but a minimal robots.txt pointing to the sitemap is good practice. Suggested:

```
User-agent: *
Allow: /

Sitemap: https://trystillpoint.life/sitemap.xml
```

Can be added via Framer Site Settings → SEO → robots.txt (if plan supports it). **Not yet done — optional next step.**

**No GSC MCP exists** in the registry — connection is not possible; Michael must view GSC data directly.

---

### 5. Legal Page and Support Page Title Tags Set

Michael set title tags for all legal pages and the support page in Framer page settings. Meta descriptions for legal pages were intentionally left blank (Google auto-generates from content — appropriate for utility pages).

**Title tags set:**
- `Privacy Policy | StillPoint`
- `Terms of Service | StillPoint`
- `Shipping Policy | StillPoint`
- `Refund Policy | StillPoint`
- `Support | StillPoint`

**Support page meta description set:**
> Have a question about StillPoint? Find answers about shipping, returns, and product care — or reach out at hello@trystillpoint.life.

---

### 6. Support Page Fully De-Templated (via Framer MCP)

The support page was identified as heavily template-based (Essence template content throughout). Reviewed via Framer MCP, and Michael updated all content fields in Framer while Claude provided exact copy.

**Before → After:**
- **Email:** `support@essence.com` → `hello@trystillpoint.life` (with correct `mailto:` link)
- **Head office:** "150 Mercer Street New York, NY 10012" → `San Anselmo, CA`
- **Phone:** "(555) 123-4567" → **completely removed** (StillPoint has no phone number)
- **Intro text:** "Do you have any questions about our products?" → "Do you have any questions about StillPoint?"
- **FAQ accordions:** Code-based components (not editable via MCP); copy was written by Claude and pasted in by Michael

**Shipping & Delivery FAQ content written:**
- When will my order ship? (pre-order, ships May 2026)
- Where do you ship from? (San Anselmo, California, USA)
- Do you ship internationally? (US only, international may come later)
- How will I know when my order has shipped? (email with tracking)

**Returns & Refunds FAQ content written:**
- What is your return policy? (30-day satisfaction guarantee, full refund)
- How do I start a return? (email hello@trystillpoint.life)
- When will I receive my refund? (original payment method, allow a few days)

**Verification:** All changes confirmed clean via Framer MCP node inspection ✅

---

### 7. Payment-Methods Page Moved to Draft

The Framer site had a payment-methods page that was a template leftover. Since all transactions go through Shopify checkout (which handles payment methods natively), this page has no function for StillPoint.

**Decision:** Michael moved the page to **draft mode** rather than deleting it.
- Off the live site and out of Google's index ✅
- Recoverable if ever needed ✅

---

## Files Added or Modified This Session

| File | Status | Notes |
|------|--------|-------|
| `claims-guardrails.md` | Modified → v2.1 | "stress relief" moved to green-light |
| `research/seo-audit-2026-04-02.md` | New | Full SEO audit, created during session |
| `session-notes-2026-04-02.md` | New (overwritten) | This file — supersedes earlier incomplete automated version |

**Framer changes (live, no local files):**
- Homepage meta description updated ("stress relief" live)
- Support page: email, address, phone, intro text, FAQ accordions all updated
- Legal page title tags set (Privacy, Terms, Shipping, Refund)
- Support page title tag and meta description set
- Payment-methods page moved to draft

---

## Pending Tasks

### High Priority
- [ ] **Rebuild Posts 01–08 at large type scale** (38px headline / 21px body / 25px closing #2a2a2a) before posting — carried from 2026-03-16; Posts 09 and 10 are approved reference files
- [ ] **Post Posts 01 and 10 to Instagram** — large-type versions ready; use Resiliencia audio for continuity
- [ ] **Fix inventory display in Framer** — "in stock" component is hidden; Frameship sync needed to show correct count (125 per size)

### Medium Priority
- [ ] **GitHub commit** — Ready to commit: `claims-guardrails.md` v2.1, `research/seo-audit-2026-04-02.md`, Instagram posts 01–10 (HTML + PNG), `instagram-following.md`
  - Suggested subjects: (1) `Update claims-guardrails to v2.1 — stress relief green-light` (2) `Add SEO audit 2026-04-02` (3) `Add Instagram post series and following list`
- [ ] **FAQPage schema markup** — Next high-value SEO action from audit; gets StillPoint into Google "People Also Ask" results
- [ ] **First blog post** — "What is a breath anchor?" would capture that keyword in search; recommended in SEO audit
- [ ] **Add robots.txt** — Optional but good practice; can be done via Framer Site Settings → SEO
- [ ] **Email nurture sequence** — `emails/preorder_warming_sequence.md` is drafted; needs review and finalization
- [ ] **Continue Instagram posting** — 5 posts live now; remaining 8 posts in series need large-type rebuild and posting

### Low Priority / Future
- [ ] **Real StillPoint product photos** — UGC strip on live site still uses Essentia placeholder photos
- [ ] **Meta Verified** — revisit at ~200–500 organic followers (currently ~7); roughly mid-May 2026
- [ ] **International shipping policy** — deferred; add when/if Michael expands beyond US
- [ ] **Trigeminal nerve claim** — flagged concern, Michael keeping as-is for now; monitor as brand scales

---

## Canon and GitHub Status

| File | Version | Status |
|------|---------|--------|
| product-canon.md | v2.0 | ✅ Committed (2026-03-12) |
| claims-guardrails.md | v2.1 | ⚠️ NOT committed — updated today |
| site-map-and-copy.md | v2.2 | ✅ Committed (2026-03-15) |
| faq-copy.md | v2.1 | ✅ Committed |
| privacy-policy.md | v1.0 | ✅ Committed (2026-03-15) |
| terms-of-service.md | v1.0 | ✅ Committed (2026-03-15) |
| shipping-policy.md | v1.0 | ✅ Committed (2026-03-15) |
| refund-policy.md | v1.0 | ✅ Committed (2026-03-15) |
| research/seo-audit-2026-04-02.md | — | ⚠️ NOT committed — new today |
| Instagram posts 01–10 (HTML) | — | ⚠️ NOT committed (since 2026-03-16) |
| Instagram PNGs 01–10 | — | ⚠️ NOT committed (since 2026-03-16) |
| instagram-following.md | — | ⚠️ NOT committed (since 2026-03-16) |

**Suggested commits when ready:**
1. Subject: `Update claims-guardrails to v2.1 — stress relief green-light`
   Description: `Moved "stress relief" from yellow-light to green-light. Approved for marketing copy and meta descriptions. "Anxiety relief" remains yellow-light.`

2. Subject: `Add SEO audit 2026-04-02`
   Description: `Full SEO audit for trystillpoint.life. Includes indexation status, keyword gaps, technical checklist, content gaps, and priority actions.`

3. Subject: `Add Instagram post series and following list`
   Description: `10 branded Instagram posts (HTML + PNG), large-type versions of posts 09 and 10, instagram-following.md target list. No canon changes.`

---

## Briefing for Next Session

Start by reading this file for full context on today's work.

The biggest thing that happened today: **trystillpoint.life is now indexed on Google.** Search Console is set up, verified, and the sitemap is submitted with 7 pages discovered. The site will surface in search results — probably within a few days to a week. This is the SEO foundation everything else builds on.

The claims guardrails are now at v2.1 with "stress relief" approved as a green-light term. That change is live in the file but not yet committed to GitHub.

The support page is fully de-templated and clean — no more Essence template content. Michael still needs to publish these Framer changes to make them live.

The two highest SEO follow-ons from the audit are: (1) **FAQPage schema markup** — a JSON-LD block that gets StillPoint questions into Google's "People Also Ask" feature, and (2) **first blog post** — "What is a breath anchor?" would own that query in search. Neither is urgent but both would meaningfully expand the site's search footprint.

The outstanding Instagram work (rebuild Posts 01–08 at large type scale, post Posts 01 and 10) remains the top carry-forward from the March 16 session. Nothing has changed there. GitHub is still uncommitted since March 16 — a clean commit sweep is overdue.

---

*Session notes written automatically at end of day, 2026-04-02.*
