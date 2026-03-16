# StillPoint Session Notes — 2026-03-16

## Session Overview
This session continued directly from 2026-03-15 notes. Primary focus was Instagram content creation: designing and producing 10 branded post images, launching the StillPoint Instagram account, and refining the visual typography system for social posts.

---

## Work Completed This Session

### 1. Instagram Post Series — All 10 Posts Created (v1 + v2)

All 10 posts were built as HTML files with an embedded caption box containing ready-to-paste Instagram captions and hashtags. Posts are saved to:
`/stillpoint/instagram/`

**The 10 Posts (v1 — original small type):**

| File | Theme | Audience |
|------|-------|----------|
| post-01-the-return.html | The return is the practice | All meditators |
| post-02-five-breaths.html | Even 5 breaths is hard | Intermediate |
| post-03-normalize-wandering.html | Wandering mind is not failure | Beginners |
| post-04-sneaky-thieves.html | Subtle undercurrent of thought | Advanced |
| post-05-goldstein-quote.html | Goldstein direct quote #1 | All |
| post-06-befriending-mind.html | Meditation as befriending | All |
| post-07-the-slope.html | Consistency over perfection | Intermediate |
| post-08-not-yet-meditator.html | Door-opener for non-meditators | Curious/new |
| post-09-what-it-is.html | Product clarity post | All |
| post-10-awakening-moment.html | Goldstein quote #2 / awakening | All |

**Design system (all posts):**
- Format: 4:5 portrait, 540×675px CSS (renders to 1080×1350px PNG at 2x)
- Background: cream #f5f2ee (Post 04 and 09 use slightly darker #f0ede8)
- Primary font: Georgia serif
- Supporting font: Helvetica Neue
- Bottom bar: "STILLPOINT" wordmark left, "trystillpoint.life" URL right
- Captions and hashtags included in each HTML file

**PNG rendering:** All 10 posts rendered as 1080×1350px PNGs using Playwright headless Chromium at device_scale_factor=2. Saved to:
`/stillpoint/instagram/png/`

**Render script:** `/sessions/brave-trusting-thompson/render_posts_hires.py`

---

### 2. Typography Refinement — Large Type System (v2)

After posting Post 01 to Instagram, Michael identified the text was too small on mobile. Research confirmed minimum 30pt body text for Instagram graphics.

**Revised type scale (approved and locked):**
- Headline: **38px CSS** (76px actual at 2x)
- Body / detail text: **21px CSS** (42px actual at 2x)
- Closing / emphasis line: **25px CSS**, color #2a2a2a (darker than body)
- Labels / eyebrow text: 13–14px CSS
- Bottom wordmark/URL: 13px CSS

**Posts rebuilt at new scale so far:**
- `post-09-what-it-is.html` ✅ — full redesign, large type, copy tightened
- `post-10-awakening-moment.html` ✅ — full redesign, large type

**Posts still needing large-type rebuild:** 01, 02, 03, 04, 05, 06, 07, 08

The approved type scale should be applied consistently to all remaining posts before they are posted to Instagram.

---

### 3. Instagram Account — Live and Active

**Account launched today.** First posts published:

1. **Video Reel (pinned)** — Screen recording of the live StillPoint website loading. Shows hero headline "Make the breath easier to feel." Duration: ~3.4 seconds. Posted as a Reel and pinned to profile as the first thing visitors see.

2. **Post 09 — What It Is** — Published ✅ (large type v2 version used)

3. **Posts 01 and 10** — Planned for today, in progress at end of session.

**Posting strategy agreed:**
- Post 09 first (product clarity), then Post 01 (meditative/poetic), then Post 10 (Goldstein closer)
- All three use **Resiliencia by Rantseni** as the background audio for continuity
- After all three are posted: follow 20–40 accounts in the meditation/mindfulness world
- Do NOT mass follow — Instagram may throttle new accounts for this

**Follow target categories:**
- Insight/Vipassana teachers: Joseph Goldstein, Tara Brach, Sharon Salzberg, Jack Kornfield, Sebene Selassie
- Meditation centers: Spirit Rock, IMS, Ten Percent Happier
- Mindfulness-adjacent wellness brands (non-competing)
- Calm productivity / focus accounts

---

### 4. Instagram Music Research

Researched top tracks for mindfulness/wellness Instagram content. Top 5 findings:

1. **"Weightless" — Marconi Union** — Scientifically proven most relaxing track (65% cortisol reduction). Available in Instagram music library. Best for first Reel.
2. **"Resiliencia" — Rantseni** — Currently trending for calm/reflective Reels (early 2026). Chosen for Posts 09, 01, 10 series.
3. **"Only Time" — Enya** — Perennial classic, keeps cycling back as trending on Reels.
4. **Moby ambient library** — Free for wellness use, but check commercial licensing since StillPoint is a brand with a buy link.
5. **"Fever Dream" — Alex Warren** — Warmer, more contemporary. Good for lifestyle/product posts.

**Important note:** Business accounts may find some tracks grayed out. Filter Instagram music library by "No restrictions" for brand-safe options.

---

### 5. Meta Verified Research

Michael received a $1/first month Meta Verified offer via Instagram pop-up.

**Research findings:**
- Independent tests show 17–30% engagement lift for verified profiles
- Benefits come primarily from trust signal (humans trust verified accounts more), not pure algorithm boost
- Regular price: $14.99–$27.99/month after intro period

**Recommendation given:** Wait 60 days. At zero followers, the badge has no audience to work on. Build to 200–500 organic followers first, then consider verification. The trust signal matters most when people are already finding you.

---

### 6. File Rendering Infrastructure

**Playwright headless Chromium** installed and working in the session environment.

Key scripts:
- `render_posts_hires.py` — renders all 10 posts at 1080×1350
- `render_single.py` — renders a single post by name (used for iteration)

**To re-render all posts:** Run `python3 /sessions/brave-trusting-thompson/render_posts_hires.py`
**To render one post:** Edit `render_single.py` post name, then run it.

---

## Files Added or Modified This Session

### New files:
- `/stillpoint/instagram/post-01-the-return.html`
- `/stillpoint/instagram/post-02-five-breaths.html`
- `/stillpoint/instagram/post-03-normalize-wandering.html`
- `/stillpoint/instagram/post-04-sneaky-thieves.html`
- `/stillpoint/instagram/post-05-goldstein-quote.html`
- `/stillpoint/instagram/post-06-befriending-mind.html`
- `/stillpoint/instagram/post-07-the-slope.html`
- `/stillpoint/instagram/post-08-not-yet-meditator.html`
- `/stillpoint/instagram/post-09-what-it-is.html` (rebuilt v2 large type)
- `/stillpoint/instagram/post-10-awakening-moment.html` (rebuilt v2 large type)
- `/stillpoint/instagram/png/post-01-the-return.png` through `post-10-awakening-moment.png`
- `/stillpoint/research/goldstein-dharma-talk-analysis.md` (created prior session, referenced here)
- `/stillpoint/session-notes-2026-03-16.md` (this file)

---

## Pending Tasks (carry into next session)

### High Priority
- [ ] **Rebuild Posts 01–08 at large type scale** (38px headline / 21px body / 25px closing) before posting
- [ ] **Post Post 01 — The Return** to Instagram with Resiliencia audio
- [ ] **Post Post 10 — The Awakening Moment** to Instagram with Resiliencia audio
- [ ] **Follow 20–40 target accounts** after all three posts are live

### Medium Priority
- [ ] **Email nurture sequence** — "Stay close to the breath" signup form is live on the website. First email and full sequence not yet written. Draft exists in `/stillpoint/emails/preorder_warming_sequence.md` — needs review and finalization.
- [ ] **GitHub commit** for all Instagram files (this session's work)

### Lower Priority / Future
- [ ] **Real StillPoint product photos** — UGC strip on live site still uses Essentia placeholder photos
- [ ] **Meta Verified** — revisit in ~60 days once account has organic followers
- [ ] **International shipping policy** — deferred; add when/if Michael expands beyond US
- [ ] **Trigeminal nerve claim** — flagged, keeping as-is, monitor as brand scales

---

## Canon and GitHub Status

**Canon version:** v2.2 (last committed prior session)
**Legal pages:** All at v1.0 (privacy policy, terms of service, shipping policy, refund policy) — committed prior session
**Instagram files:** NOT YET COMMITTED — ready to commit this session

**GitHub commit ready:**
- Subject: `Add Instagram post series — all 10 posts (HTML + PNG)`
- Description: `Created 10 branded Instagram posts as HTML files with captions and hashtags. Rendered all 10 as 1080x1350px PNGs. Posts 09 and 10 rebuilt at large-type scale (38px headline / 21px body). Added render scripts. Added Goldstein dharma talk research analysis.`

---

## Briefing for Next Session

Start by reading this file and session-notes-2026-03-15.md for full context.

The most important thing to do at the start of the next session is **rebuild Posts 01–08 at the approved large-type scale** before any more are posted to Instagram. The type system is now locked:
- Headline: 38px
- Body: 21px
- Closing/emphasis: 25px, color #2a2a2a

Post 09 (live, large type ✅) and Post 10 (ready, large type ✅) are the approved reference files. All remaining posts should match their sizing system exactly.

Instagram is live at the StillPoint account. The pinned video Reel is up. Post 09 has been posted. Posts 01 and 10 are next in queue.

The email nurture sequence is the next major content project after Instagram posts are complete.
