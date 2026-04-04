# StillPoint Session Notes — 2026-04-03

**Session type:** SEO completion + Instagram + PR gifting system + care instructions
**Canon additions:** `care-instructions.md` v1.0 (new)
**GitHub status:** Several new/updated files ready to commit — see below

---

## Session Overview

A full, productive day. Started by reviewing yesterday's session notes to establish what had already been done, then swept through the remaining SEO action items. Both open items were completed: the homepage title tag was verified live, and JSON-LD Product schema was written, deployed, and confirmed. FAQPage schema was also added in the same session, bringing the site to four structured data blocks. Then moved into Instagram, PR gifting infrastructure, and care instructions. New operational files created: `ideas.md`, `pr-gifting-list.md`, and `canon/care-instructions.md`.

---

## Work Completed This Session

### 1. SEO — Homepage Title Tag and Meta Description Verified Live

Confirmed both are correctly published on trystillpoint.life via Chrome MCP page inspection:

- **Title:** `StillPoint™ | Nose-Worn Breath Awareness Meditation Device` ✅
- **Meta description:** `StillPoint is a handcrafted, nose-worn breath anchor that makes the breath easier to feel — supporting meditation, stress relief, and sleep. First Batch available now.` ✅

Both were set a few days prior — this session confirmed they are live and correct.

---

### 2. SEO — JSON-LD Product Schema Deployed

Written and deployed to Framer Site Settings → Custom Code → `<head>`. Verified live via page source inspection.

**Schema fields:** Product name (StillPoint Air), description, brand (StillPoint), URL, price ($24.00 USD), availability (PreOrder), seller.

Confirmed present and correctly formed in page source ✅

---

### 3. SEO — FAQPage Schema Deployed

A second JSON-LD block added to the same `<head>` section immediately after the Product schema. 7 questions selected from `faq-copy.md` for highest "People Also Ask" relevance.

**Questions included:**
- Does StillPoint block breathing?
- Does StillPoint go inside the nostrils?
- Is StillPoint a nasal dilator?
- How does StillPoint stay on?
- Is StillPoint a medical device?
- Can I wear StillPoint at bedtime?
- What is StillPoint's return policy?

Confirmed live — all 7 questions parsing correctly ✅

Site now has 4 structured data blocks: Product, FAQPage, Organization, WebSite (Organization and WebSite are Framer-generated).

---

### 4. Ideas Log Created

New file created: `/stillpoint/ideas.md` — running log for marketing ideas and future initiatives. Not a task list; a capture system for things worth remembering.

**Ideas logged today:**
- Mindfulness podcast outreach (interview / sponsorship)
- Truck poster with QR code linking to trystillpoint.life
- Contact The Sleep Doctor (Dr. Michael Breus) — send a device once packaging ready
- Welcome page (trystillpoint.life/welcome) — QR code landing page for new customers, Second Batch build

---

### 5. Instagram Following List — Rebuilt and Authoritative

`instagram/instagram-following.md` fully rebuilt from live Instagram data provided by Michael. Profile now shows 159 following, 13 followers, 7 posts.

**Going forward:** Always check this file before generating new follow suggestions to prevent duplicates.

**Handle corrections noted this session:**
| Wrong | Correct |
|---|---|
| @davidji_meditation | @davidjimeditation |
| @leeharrisofficial | @leeharrisenergy |
| @michaelsingerauthor | @michael_a.singer |
| @pemachodronofficial | @anipemachodron |
| @dr.beckykennedy | @drbeckyatgoodinside |
| @markdivine | @markdivineofficial |
| @rodneyyee | @rodneyyeeyoga |
| @yogawithkassandra | @yoga_with_kassandra |

**Previously thought unresolvable, now confirmed following:** @timferris

---

### 6. PR Gifting List Created

New file: `research/pr-gifting-list.md` — master operational list of people to receive a StillPoint device once packaging is finalized and First Batch ships.

**Currently on the list:**
- 7 wellness editor contacts (from `pr-outreach-2026.md`): Mindful Magazine, Well+Good, Yoga Journal (×2), mindbodygreen, Lion's Roar, Breathe Magazine
- Dr. Michael Breus (@thesleepdoctor) — sleep expert, strong product fit

Mailing addresses are TBD — to be researched before May. April 23 reminder already set to initiate shipping prep.

---

### 7. Care Instructions Written — Three Versions

New canon file created: `canon/care-instructions.md` v1.0

Material: TPU (Thermoplastic Polyurethane). Key real-world note: dish soap leaves residue if not rinsed thoroughly — the rinsing step is critical for a device worn at the nose.

**Three versions written:**
- **Welcome page version** — concise, brand-voiced, closes with "That's it."
- **Product card version** — condensed single-paragraph for the package insert
- **Support page version** — full version with disinfecting instructions, what to avoid, and storage notes

**Placement decision:**
- Primary home: Welcome page (trystillpoint.life/welcome) — linked via QR code on packaging
- Future: Detailed support page section in next site update
- Product card insert: condensed version

---

## Files Added or Modified This Session

| File | Status | Notes |
|------|--------|-------|
| `session-notes-2026-04-03.md` | Modified | This file |
| `ideas.md` | New | Running ideas log — 4 ideas captured |
| `instagram/instagram-following.md` | Rebuilt | Authoritative list from live Instagram data; 159 following |
| `research/pr-gifting-list.md` | New | Master PR gifting list — 8 contacts, addresses TBD |
| `canon/care-instructions.md` | New | v1.0 — three versions of care copy |

**Framer changes (live, no local files):**
- JSON-LD Product schema added to `<head>`
- FAQPage schema added to `<head>`

---

## Pending Tasks

### High Priority
- [ ] **Rebuild Posts 01–08 at large type scale** (38px headline / 21px body / 25px closing #2a2a2a) — Posts 09 and 10 are reference files
- [ ] **Post to Instagram** — large-type versions ready; use Resiliencia audio for continuity
- [ ] **Fix inventory display in Framer** — "in stock" component hidden; Frameship sync needed

### Medium Priority
- [ ] **GitHub commit sweep** — uncommitted: `claims-guardrails.md` v2.1, `research/seo-audit-2026-04-02.md`, `ideas.md`, `instagram/instagram-following.md`, `research/pr-gifting-list.md`, `canon/care-instructions.md`, Instagram posts 01–10 (HTML + PNG), `instagram-following.md`
- [ ] **Research mailing addresses** for PR gifting list before May — publication offices, Dr. Breus contact
- [ ] **Email nurture sequence** — `emails/preorder_warming_sequence.md` drafted; needs review and finalization
- [ ] **First blog post** — "What is a breath anchor?" — recommended in SEO audit
- [ ] **Add robots.txt** — optional but good practice; Framer Site Settings → SEO
- [ ] **Add care instructions to support page** — full version from `canon/care-instructions.md`

### Low Priority / Future (Second Batch)
- [ ] **Welcome page** — trystillpoint.life/welcome, QR code landing, how to wear + what to expect + care instructions; copy ready in `canon/care-instructions.md`
- [ ] **Real StillPoint product photos** — UGC strip still uses Essentia placeholder photos
- [ ] **Meta Verified** — revisit at ~200–500 followers; mid-May 2026 estimate
- [ ] **Mindfulness podcast outreach** — interview / commercial spot; log in `ideas.md`
- [ ] **Truck poster with QR code** — local awareness play; log in `ideas.md`

---

## Canon and GitHub Status

| File | Version | Status |
|------|---------|--------|
| product-canon.md | v2.0 | ✅ Committed |
| claims-guardrails.md | v2.1 | ⚠️ NOT committed |
| site-map-and-copy.md | v2.2 | ✅ Committed |
| faq-copy.md | v2.1 | ✅ Committed |
| care-instructions.md | v1.0 | ⚠️ NOT committed — new today |
| research/seo-audit-2026-04-02.md | — | ⚠️ NOT committed |
| research/pr-gifting-list.md | — | ⚠️ NOT committed — new today |
| ideas.md | — | ⚠️ NOT committed — new today |
| instagram/instagram-following.md | — | ⚠️ NOT committed — rebuilt today |
| Instagram posts 01–10 (HTML + PNG) | — | ⚠️ NOT committed (since 2026-03-16) |

---

## Briefing for Next Session

Strong day. The SEO foundation is complete — title tag, meta description, Product schema, and FAQPage schema are all live and verified. The site is indexed, structured data is in place, and Google has everything it needs to start surfacing StillPoint in search results and potentially in "People Also Ask."

On the operational side, three new infrastructure files were created today: `ideas.md` (running ideas capture), `pr-gifting-list.md` (master gifting/outreach list for May shipping), and `canon/care-instructions.md` (three-version care copy ready to deploy). The Instagram following list is now authoritative and rebuilt from live data — use it as the reference for all future follow suggestions.

The most overdue item is the GitHub commit sweep — a significant backlog has accumulated. That's a clean, low-risk task for any session. The Instagram posting work (large-type Posts 01–08 rebuild) remains the top creative carry-forward.

April 23 reminder is set for PR gifting prep. Mailing addresses for the gifting list need to be researched before May.

---

*Session notes written 2026-04-03.*
