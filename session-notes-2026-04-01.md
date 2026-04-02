# StillPoint Session Notes — 2026-04-01

**Session type:** Project re-orientation + automation setup + Instagram content + Framer product page work
**Canon version:** v2.2 (unchanged — no new canon commits today)
**GitHub status:** NOT committed — Instagram files and recent work remain uncommitted since 2026-03-16

---

## Session Overview

Two sessions today. The primary session ("Review StillPoint project folder") opened with a full project review to re-establish context, then covered three areas: setting up an automated session notes + morning briefing system, creating and publishing a new Instagram post from an original product photo, and a discussion of Instagram link strategy and Gmail dispatch limitations.

A secondary session ("Write sizing accordion copy for StillPoint") — likely earlier today or March 31 — addressed product page improvements in Framer: sizing accordion copy, default variant fix, and an inventory display issue.

---

## Work Completed This Session

### 1. Automated Session Notes + Morning Briefing System

Two scheduled tasks were created and are now running:

- **10 PM daily — Session notes:** Automatically reviews the day's transcript and writes a formatted `session-notes-YYYY-MM-DD.md` file to the StillPoint project folder (this file).
- **7 AM daily — Morning briefing:** Fires a summary of yesterday's work, open threads, and today's priorities.

Both tasks are visible in the Scheduled section of the sidebar and can be paused, edited, or triggered manually.

---

### 2. Instagram Post — Lavender/Flowers Product Photo

New post created and published to @stillpointdevice.

**Photo:** StillPoint device held in hand next to purple/lavender flowers. Iridescent material catching warm light.

**Song:** "All My Favorite Colors" — chosen by Michael.

**Caption development:** Three options were drafted. Option B was selected and developed into a full post:

> All your favorite colors were always here.
>
> Still Point is a small reminder that presence is, too.
>
> Soft. External. Worn on the nose. It makes the breath easier to feel — so attention can return, naturally, to whatever is right in front of you.
>
> Pre-order open · link in bio 🤍

**Hashtags:** #stillpoint #breathawareness #meditationtools #mindfulmoments #breathwork #presentmoment #meditationpractice #consciousliving #slowdown #sensorypresence #mindbody #breathe #wellnesstools #mindfulbreathing #stopandsmelltheflowers #somaticwellness #gentleliving #embodiedpresence #nervoussystemhealth #naturephotography

**Status:** Published ✅ — confirmed by Michael ("posted!")

**Link strategy confirmed:** Instagram captions do not support clickable links. The bio link (`trystillpoint.life`) is the only clickable entry point. Caption practice: write "link in bio" and let the bio handle the click-through. No changes needed — bio is already set correctly.

---

### 3. Instagram Pinning Instructions

Michael asked how to pin a post on Instagram. Answered:

- Go to profile → tap the post → three dots (⋯) → "Pin to your profile"
- Up to 3 posts can be pinned; pinned posts appear at top of grid with a pin icon
- To unpin: same flow → "Unpin from your profile"

---

### 4. Gmail Dispatch Limitations Confirmed

Michael asked about being contacted via Gmail while away ("dispatch function"). Clarified:

- Gmail MCP supports **draft creation only** — it cannot send emails
- Not suitable for real-time dispatch or push notifications
- Best approach for now: check back in the conversation when available; scheduled tasks run automatically regardless

---

### 5. Product Page Work — Framer (Prior Session, ~March 31)

The following work was completed in a session titled "Write sizing accordion copy for StillPoint." Based on session list order, this was likely March 31 or earlier today.

**Sizing accordion added to product page:**
- Three sections written: Small, Medium, Large (with overlap reassurance copy between sizes)
- Accordion placed above the Shipping and Return Policy section on the Framer product page
- Implemented via Framer MCP (no local file)

**Default variant fixed — Medium is now default:**
- Product page was defaulting to Small on load
- Root cause: Frameship plugin had cached Shopify variant order (Small first) in Framer's VariantSelector component
- Fix: Michael synced the Frameship plugin in Framer's CMS settings — this pulled the updated variant order from Shopify and set Medium as default
- **Architecture note confirmed:** Framer is the live storefront; Shopify is the backend. Frameship plugin caches Shopify data inside Framer. Changes in Shopify don't propagate automatically — Frameship sync is required for variant/inventory data.

**Inventory count issue — temporarily resolved by hiding:**
- "50 in stock" text was displaying stale Frameship data; actual inventory is 125 per size in Shopify
- Correct fix: Frameship sync on the inventory display component
- Michael hid the component as a quick fix rather than debug further
- Still needs proper resolution (see Pending Tasks)

---

## Files Added or Modified This Session

| File | Status | Notes |
|------|--------|-------|
| `session-notes-2026-04-01.md` | New | This file |
| Instagram post — lavender/flowers | Published | Live on @stillpointdevice, no local file |
| Sizing accordion (Framer) | Modified in Framer | Added via Framer MCP, no local file to commit |
| Scheduled tasks | Created | Session notes (10 PM) + briefing (7 AM) — internal Cowork infrastructure |

**Note:** No new local files were written to the StillPoint project folder during today's primary session. Framer product page changes were made directly in Framer via MCP.

---

## Pending Tasks

### High Priority
- [ ] **Rebuild Posts 01–08 at large type scale** (38px headline / 21px body / 25px closing #2a2a2a) before posting — carried from 2026-03-16
- [ ] **Fix inventory display in Framer** — "in stock" component is hidden; Frameship sync on that component needed to show correct count (125 per size)
- [ ] **Post Posts 01 and 10 to Instagram** — carried from 2026-03-16; both have large-type versions ready

### Medium Priority
- [ ] **GitHub commit** — Nothing committed since 2026-03-16. Ready to commit: Instagram posts 01–10 (HTML + PNG), `instagram-following.md`, any other new files
- [ ] **Email nurture sequence** — `emails/preorder_warming_sequence.md` is drafted; needs review and finalization
- [ ] **Continue Instagram posting** — 5 posts live now (including today's lavender/flowers post); series of 10 should be posted with Resiliencia audio where appropriate

### Low Priority / Future
- [ ] **Real StillPoint product photos** — UGC strip on live site still uses Essentia placeholder photos
- [ ] **Meta Verified** — revisit at ~200–500 organic followers (currently ~7); originally suggested at 60 days, roughly mid-May 2026
- [ ] **International shipping policy** — deferred; add when/if Michael expands beyond US
- [ ] **Trigeminal nerve claim** — flagged concern, Michael keeping as-is for now; monitor as brand scales

---

## Canon and GitHub Status

| File | Version | Status |
|------|---------|--------|
| product-canon.md | v2.0 | ✅ Committed (2026-03-12) |
| claims-guardrails.md | v2.0 | ✅ Committed (2026-03-12) |
| site-map-and-copy.md | v2.2 | ✅ Committed (2026-03-15) |
| faq-copy.md | v2.1 | ✅ Committed |
| privacy-policy.md | v1.0 | ✅ Committed (2026-03-15) |
| terms-of-service.md | v1.0 | ✅ Committed (2026-03-15) |
| shipping-policy.md | v1.0 | ✅ Committed (2026-03-15) |
| refund-policy.md | v1.0 | ✅ Committed (2026-03-15) |
| Instagram posts 01–10 (HTML) | — | ⚠️ NOT committed |
| Instagram PNGs 01–10 | — | ⚠️ NOT committed |
| instagram-following.md | — | ⚠️ NOT committed |

**Suggested commit when ready:**
- Subject: `Add Instagram post series and following list`
- Description: `10 branded Instagram posts (HTML + PNG), large-type versions of posts 09 and 10, instagram-following.md target list. No canon changes.`

---

## Briefing for Next Session

The automated session notes and morning briefing are now live — this file was written by the 10 PM scheduled task. Start future sessions by reading the most recent session notes file.

The Instagram account is at 5 posts (product clarity post 09, lavender/flowers post today, and the pinned opening Reel). The remaining 9 posts from the original series (01–10) still need large-type rebuilds before posting — this is the highest carry-forward priority from March 16. Post 09 (large type ✅) and Post 10 (large type ✅) are the approved reference files for type scale.

The Framer product page is cleaner than before: sizing accordion added, Medium is default. The "50 in stock" text is hidden but the underlying Frameship sync issue hasn't been resolved — worth a quick fix early next session.

No GitHub commits since 2026-03-16. The Instagram HTML/PNG files and following list are ready to commit whenever Michael is ready to push.

The email nurture sequence (`emails/preorder_warming_sequence.md`) is drafted and waiting. That's the next major content project after the Instagram post series is complete.

---

*Session notes written automatically at 10 PM, 2026-04-01.*
