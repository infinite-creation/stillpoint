# StillPoint Session Notes — 2026-04-04

**Session type:** Post-SEO follow-through + operational infrastructure — FAQPage schema, ideas log, Instagram list rebuild, PR gifting list, care instructions
**Canon version at end of session:** No canon changes today
**GitHub status:** Nothing new to commit from today's session (new files are operational/research, not canon)

---

## Session Overview

This session continued directly from the "Product page SEO setup tasks" session that had begun on April 3. The April 3 10 PM auto-generated notes captured the Product schema work done earlier that day; today's notes cover the work that happened after that — starting with the FAQPage schema and running through Instagram infrastructure, PR gifting list creation, and care instruction drafting.

Six areas of work: FAQPage schema deployed, ideas log created, Instagram following list rebuilt from live data, PR gifting list created, and care instruction copy written for the welcome page and product card.

---

## Work Completed This Session

### 1. FAQPage Schema — Written and Deployed

Wrote and deployed a 7-question FAQPage JSON-LD schema block in Framer Site Settings → Custom Code → `<head>`, alongside the existing Product schema. Verified live via page inspection.

**Questions included:**
1. Does StillPoint block breathing?
2. Does StillPoint go inside the nostrils?
3. Is StillPoint a nasal dilator?
4. How does StillPoint stay on?
5. Is StillPoint a medical device?
6. Can I wear StillPoint at bedtime?
7. What is StillPoint's return policy?

**Status:** ✅ Live on trystillpoint.life — all 7 questions parsing correctly

**Note:** Framer is also automatically injecting Organization and WebSite schemas on its own. The site now has 4 structured data blocks total. FAQPage schema will take time for Google to pick up; once indexed, these questions become candidates for "People Also Ask" results in search.

---

### 2. Ideas Log — Created

Created `ideas.md` in the root of the StillPoint project folder. A simple, date-stamped running file for ideas that come up during sessions — not commitments, just things worth remembering.

**Location:** `/stillpoint/ideas.md`

**Initial ideas logged (all 2026-04-03):**
- **Mindfulness podcast outreach** — Reach out to mindfulness podcasts about being interviewed on StillPoint's creation and the product itself. Could explore paid commercial spots over time.
- **Truck poster with QR code** — Large printed poster for the back of Michael's truck with QR code linking to trystillpoint.life. Low-cost, high-visibility local awareness.
- **Contact Dr. Michael Breus (@thesleepdoctor)** — Send a device once packaging is finalized. Strong fit: sleep is a core StillPoint use case. Linked to PR gifting list.

**Usage note:** Going forward, ideas that come up in session can be logged here on request. Periodically reviewable via morning briefing or on demand.

---

### 3. Instagram — Batch 4 Follow Candidates Researched

Generated a list of 30 new follow candidates across categories: meditation teachers, breathwork, sleep science, health/longevity, yoga, apps, organizations, somatic practitioners.

**Corrected handles (from Michael's Instagram data):**
| Suggested | Correct |
|-----------|---------|
| @davidji_meditation | @davidjimeditation |
| @leeharrisofficial | @leeharrisenergy |
| @michaelsingerauthor | @michael_a.singer |
| @pemachodronofficial | @anipemachodron |
| @dr.beckykennedy | @drbeckyatgoodinside |

**Previously followed accounts that appeared in Batch 4 (excluded):** @jamesclear, @drmattwalker, @peterattiamd

**Note:** Michael provided a live export of the full Instagram following list (159 accounts). That data was used to rebuild the canonical reference file — see item 4.

---

### 4. Instagram Following List — Fully Rebuilt from Live Data

The `instagram-following.md` file was completely rebuilt from Michael's live Instagram following export (159 accounts as of this session). The file is now the authoritative canonical reference.

**Going forward:** Before generating any new follow suggestions, the canonical list will be checked to prevent duplicate recommendations. This directly addresses the redundancy problem Michael flagged.

**Current account stats:** 7 posts · 13 followers · 159 following

---

### 5. PR Gifting List — Created

Created `research/pr-gifting-list.md` — a master operational list of people to receive a StillPoint device once First Batch packaging is finalized and ships (May 2026).

**Location:** `/stillpoint/research/pr-gifting-list.md`

**Structure:** Two sections — Wellness Editors (Publications) and Sleep & Health Experts. Each row tracks: name, publication/role, email, mailing address (TBD for most), notes, and status.

**Contents (8 recipients):**
- Amber Tucker / Ava Whitney-Coulter — Mindful Magazine
- Frankie Krempa — Well+Good (commerce editor; send 2 units)
- Ellen O'Brien — Yoga Journal
- Tamara Jeffries — Yoga Journal (secondary contact)
- Editorial — mindbodygreen
- Editorial — Lion's Roar
- Editorial — Breathe Magazine (UK — flag international shipping)
- Dr. Michael Breus — The Sleep Doctor (@thesleepdoctor)

**Note:** Mailing addresses are TBD for all recipients — should be researched before May. The April 23 reminder (already set) covers initiating this outreach along with the wellness editors.

---

### 6. Care Instructions — Researched and Drafted

Researched TPU cleaning best practices using Michael's Google research + material science context. Drafted care instructions in two formats.

**Key finding from Michael's own experience:** Dish soap leaves surfactant residue noticeable on a nose-worn device. Instructions explicitly call out thorough rinsing.

**Welcome page copy (approved):**
> After each use, rinse gently with warm water. For a deeper clean, add a small drop of mild dish soap, work it lightly with your fingertips, and rinse thoroughly under warm running water — take a moment to make sure all soap is fully cleared. Let it air dry completely before wearing or storing.
>
> Avoid bleach, vinegar, and alcohol-based sprays. Don't soak.
>
> That's it.

**Product card insert copy (condensed):**
> Rinse with warm water after use. For a deeper clean, wash with mild dish soap and rinse thoroughly — make sure all soap is cleared. Air dry fully. Avoid bleach and alcohol sprays.

**Placement decided:**
- Welcome page (`trystillpoint.life/welcome`) — full copy above; this is a Second Batch build
- Product card insert — condensed version
- Support page (future) — more detailed, searchable version when the support page is expanded

**Status:** Copy drafted and approved in conversation; not yet saved to a file. See Pending Tasks.

---

## Files Added or Modified This Session

| File | Status | Notes |
|------|--------|-------|
| `ideas.md` | ✅ New | Running ideas log; 3 initial entries |
| `research/pr-gifting-list.md` | ✅ New | Master PR gifting list; 8 recipients, all TBD on addresses |
| `research/instagram-following.md` | ✅ Updated | Fully rebuilt from live Instagram data; 159 accounts, now canonical |

No Framer changes required a file; the FAQPage schema lives in Framer Custom Code (`<head>`).

---

## Pending Tasks

### High Priority
- [ ] **Rebuild Posts 01–08 at large type scale** (38px headline / 21px body / 25px closing #2a2a2a) before posting — carried since 2026-03-16; Posts 09 and 10 are approved reference files
- [ ] **Post Posts 01 and 10 to Instagram** — large-type versions ready; use Resiliencia audio for continuity
- [ ] **Fix inventory display in Framer** — "in stock" component is hidden; Frameship sync needed to show correct count (125 per size)
- [ ] **Save care instructions to file** — welcome page copy and product card copy both approved in session but not yet written to `/stillpoint/canon/` or a dedicated `care-instructions.md` file

### Medium Priority
- [ ] **Research mailing addresses** for all 8 PR gifting list recipients before May — see `research/pr-gifting-list.md`
- [ ] **GitHub commit** — ready to commit: `claims-guardrails.md` v2.1, `research/seo-audit-2026-04-02.md`, Instagram posts 01–10 (HTML + PNG), `instagram-following.md` (rebuilt), `research/pr-gifting-list.md`, `ideas.md`
- [ ] **First blog post** — "What is a breath anchor?" would capture that keyword in search; recommended in SEO audit
- [ ] **Add robots.txt** — Optional but good practice; can be done via Framer Site Settings → SEO
- [ ] **Email nurture sequence** — `emails/preorder_warming_sequence.md` is drafted; needs review and finalization
- [ ] **Continue Instagram posting** — remaining posts in series need large-type rebuild and posting; use rebuilt `instagram-following.md` as reference going forward

### Low Priority / Future
- [ ] **Welcome page build** (`trystillpoint.life/welcome`) — QR code destination for post-purchase; cover how to wear, what to expect, and care instructions; this is a Second Batch project
- [ ] **Real StillPoint product photos** — UGC strip on live site still uses Essentia placeholder photos
- [ ] **Meta Verified** — revisit at ~200–500 organic followers (currently ~13); roughly mid-May 2026
- [ ] **International shipping policy** — deferred; add when/if StillPoint expands beyond US
- [ ] **Trigeminal nerve claim** — flagged concern, Michael keeping as-is for now; monitor as brand scales

---

## Canon and GitHub Status

| File | Version | Status |
|------|---------|--------|
| product-canon.md | v2.0 | ✅ Committed |
| claims-guardrails.md | v2.1 | ⚠️ NOT committed |
| site-map-and-copy.md | v2.2 | ✅ Committed |
| faq-copy.md | v2.1 | ✅ Committed |
| research/seo-audit-2026-04-02.md | — | ⚠️ NOT committed |
| Instagram posts 01–10 (HTML + PNG) | — | ⚠️ NOT committed (since 2026-03-16) |
| research/instagram-following.md | — | ⚠️ NOT committed (rebuilt this session) |
| research/pr-gifting-list.md | — | ⚠️ NOT committed (new this session) |
| ideas.md | — | ⚠️ NOT committed (new this session) |

---

## Briefing for Next Session

The SEO foundation is complete: site indexed, title tag live, Product schema live, FAQPage schema live (4 structured data blocks total). No further SEO work needed in the near term — Google will pick up the FAQPage schema over the coming days.

The two most important things to start next session:

1. **Save the care instructions to a file** — both the welcome page version and the product card version were approved in conversation but never written to disk. A 2-minute task. Suggested path: `canon/care-instructions.md` with clearly labeled sections for each use case.

2. **Begin the large-type Instagram rebuild** — Posts 01–08 still need to be rebuilt at the approved type scale (38px headline / 21px body / 25px emphasis) before they can be posted. Posts 09 and 10 are the reference. This is the longest-standing carry-forward in the project.

PR gifting infrastructure is now solid: the gifting list exists, the reminder is set for April 23, and the ideas log is in place. The main operational gap before May is researching mailing addresses for the 8 recipients.

The Instagram following list is now canonical and clean. When Michael wants a new batch of follow suggestions, the rebuilt file will be checked first.

---

*Session notes written 2026-04-04 (automated).*
