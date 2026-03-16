# StillPoint Session Notes — 2026-03-15 (Sunday)

**Session type:** Live site review follow-up + pre-order copy finalization + full legal pages build-out
**Canon version at end of session:** site-map-and-copy.md v2.2 / faq-copy.md v2.1 / product-canon.md v2.0 / claims-guardrails.md v2.0 / all legal pages v1.0
**GitHub status:** All updates committed and pushed ✅

---

## What we accomplished today

### 1. Live site confirmed clean — screenshots reviewed

Michael shared screenshots of the updated live site at trystillpoint.life. Confirmed:
- "Reserve Yours" button live in nav and as mid-page CTA ✅
- Pre-order notice live in buy block: "This is a pre-order. First Batch is 400 units, handcrafted in the USA. Ships May 2026." ✅
- Buy block description initially still showed "leaving airflow unobstructed" — confirmed this was because Framer and Shopify ARE connected; once Shopify was updated, the change propagated to the Framer site automatically. Key workflow note: **edit product description in Shopify → it flows to Framer live site.**
- New hand photo in hero — beautiful addition

### 2. Buy block description finalized and live

**Approved final description (v2.2):**
> StillPoint is a soft, external breath anchor worn on the nose that makes the breath easier to feel at the nostrils—so attention can focus and also return naturally. It rests gently on the outer nasal sidewalls and intentionally floats around the nasal tip, quietly redirecting airflow to make the breath more vivid at and around the nostrils. No apps. No tracking. No batteries—just a quiet, tactile cue for meditation, transitions between tasks, and bedtime wind-down. Individual experiences vary.

Key change from v2.1: "focus and also return naturally" (Michael's addition — names both the focusing and the returning). Pasted into Shopify and confirmed live on Framer site.

### 3. Canon updated to v2.2

site-map-and-copy.md updated to v2.2:
- "Reserve Yours" button documented as approved CTA (replaces "Buy Now")
- Pre-order notice documented as approved copy
- Buy block description updated with "focus and also return naturally"
- Changelog updated

**GitHub commit made:**
- Subject: `Canon v2.2 — pre-order copy, Reserve Yours button, buy block description update`
- Committed and pushed ✅

### 4. Copy button issue noted

The "Copy plain text for Shopify" button in HTML files did not work — the clipboard API requires HTTPS and doesn't function with locally opened files. Going forward: plain text will be pasted directly into the chat for easy copying. HTML formatted versions are still useful for reading/reviewing but the copy button approach has been retired.

### 5. Full legal pages built and committed

All four legal pages created from scratch or customized from Shopify templates, saved to canon, pasted into Shopify and live on website.

#### Decisions applied consistently across all legal pages:
- Contact email: **hello@trystillpoint.life** (not michael@goinginward.life)
- Address: **San Anselmo, CA, USA** (no street address — privacy preference)
- No phone number (email-only)
- No VAT number (not applicable)
- No business registration number (sole proprietor)

#### privacy-policy.md — v1.0
Custom policy written from scratch in StillPoint's voice. Covers data collection, Shopify as processor, cookies, user rights, GDPR/UK, children's data, security, and contact. Clean, warm, human. Saved to canon and live on site and Shopify.

#### terms-of-service.md — v1.0
Customized from Shopify's 25-section template. All sections preserved intact (especially Section 9 — Shopify relationship, which must not be modified). All [INSERT] placeholders filled. michael@goinginward.life replaced with hello@trystillpoint.life throughout. Phone, business registration, and VAT fields removed. Saved to canon and live on site and Shopify.

#### shipping-policy.md — v1.0
Written from scratch. Originally included international shipping section — removed at Michael's direction. US-only for First Batch pre-order launch. International shipping to be added later if/when Michael decides to expand. Key contents: pre-order ship date (May 2026), free US standard shipping (3–5 days), expedited option, address accuracy, lost packages. Saved to canon and live on Shopify.

#### refund-policy.md — v1.0
Finalized from earlier session draft. Unique destroy-and-photograph return process: customer cuts device into 4 pieces, photos it, emails the photo, receives full refund — no return shipping required. Rationale: personal care item worn on nose, can't be restocked or resold. Includes: damages/incorrect items, exchanges, sale items/gift cards, EU 14-day cooling off period. Saved to canon and live on Shopify.

**GitHub commit made:**
- Subject: `Add legal pages — privacy policy, terms of service, shipping policy`
- All three committed and pushed ✅

**GitHub commit made:**
- Subject: `Add refund-policy.md — completes legal pages canon`
- Committed and pushed ✅

### 6. Contact information set in Shopify

Michael confirmed Shopify contact info:
- Trade name: StillPoint
- Email: hello@trystillpoint.life
- Address: San Anselmo CA 94960, United States
- No phone number

### 7. Shopify main email updated

Earlier in session: Michael updated Shopify store email from michael@goinginward.life → hello@trystillpoint.life in Settings → Store details.

---

## Workflow notes confirmed this session

1. **Shopify → Framer sync:** Product description edited in Shopify propagates automatically to the live Framer site. No need to edit in Framer separately for product description.
2. **GitHub commits:** Always provide subject line + description ready to use. ✅ (established last session, confirmed this session)
3. **Copy button:** HTML file copy buttons don't work locally. Provide plain text directly in chat instead.

---

## Full canon inventory — end of session

| File | Version | Status |
|------|---------|--------|
| product-canon.md | v2.0 | ✅ Committed |
| claims-guardrails.md | v2.0 | ✅ Committed |
| site-map-and-copy.md | v2.2 | ✅ Committed |
| faq-copy.md | v2.1 | ✅ Committed |
| privacy-policy.md | v1.0 | ✅ Committed |
| terms-of-service.md | v1.0 | ✅ Committed |
| shipping-policy.md | v1.0 | ✅ Committed |
| refund-policy.md | v1.0 | ✅ Committed |

---

## Still outstanding / to monitor

1. **Social proof images** — Essentia placeholder photos still in the UGC strip on the live site. To be replaced with real StillPoint photos when available.
2. **Trigeminal nerve claim** — Live site reads "StillPoint activates the trigeminal nerve pathway." Flagged concern logged. Michael keeping as-is for now. Revisit when brand scales.
3. **International shipping** — Removed from shipping policy for First Batch. Add back when/if Michael decides to ship internationally.

---

## Pending tasks for next session

1. **Instagram and social content** — The big next horizon. Canon is locked, site is clean, legal is done. Time to build the social presence to drive pre-order traffic.
2. **Pre-order marketing push** — Strategy and content for driving awareness and reservations. 400 units to move by May 2026.
3. **Email marketing** — The email list signup ("Stay close to the breath") is live on the site. What's the first email? What's the nurture sequence?
4. **Session notes update** — Write v2.3 session notes once session notes for 2026-03-13 are updated to reflect today's decisions (minor housekeeping).

---

## Briefing paragraph for next session

The StillPoint canon is complete and fully committed at v2.2 (copy) and v1.0 (all legal pages). The live site at trystillpoint.life is clean, accurate, and pre-order ready — "Reserve Yours" button live, pre-order notice showing, buy block description updated with the correct airflow language, and all legal pages live on both Framer and Shopify. The product is StillPoint Air, $24, Ships May 2026, 400 units First Batch handcrafted in the USA. Shopify → Framer sync is confirmed working for product description. The next major work area is the pre-order marketing push — Instagram content and strategy, and potentially an email nurture sequence for people who sign up via the "Stay close to the breath" footer form.

---

*Session notes written end of day 2026-03-15.*
