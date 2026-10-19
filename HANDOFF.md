# AVR Vasthu Home 2D Plan — handoff at ~60%

**Live:** https://10elizabethbell.github.io/avrVasthuHome/ · **Repo:** https://github.com/10elizabethbell/avrVasthuHome · **Built:** 2026-10-19 from Muse brief 2026-10-19 (FB group ad, "NJ CONTRACTORS, BUILDERS & GC's")

> **First India-based prospect — flag before any outreach:** +91 country code is inferred, callbacks cross a 9.5–10.5 h time difference, and texting/WhatsApp are unconfirmed.

## What's built
- One page, single file (`index.html`), phone first: header (AVR mark + "91500 09835" tap-to-call top-right), hero, prices, how it works + service area, "Start your plan" form, footer.
- **World:** the drafting table. Blueprint-navy hero, drafting-paper sections, marigold pen/accent (auspicious marigold, Tamil Nadu). Dimension-line dividers draw in as you scroll.
- **Signature:** a Vastu floor plan (28′ × 36′, north up: pooja NE, kitchen SE, master bed SW) drafts itself wall by wall with a marigold pen tip, then doors, stairs, labels and overall dimensions; holds, fades, redraws. A finger or mouse takes the pen: drag to draw walls that snap to the 1-ft grid with a live length label (works up/down/sideways on phones; page doesn't scroll while drawing on the plan). The compass needle swings toward your finger and springs back to north.
- **Prices:** all 10 lines verbatim from the ad (Rs, not rounded/converted). Each row links to the form and pre-ticks that service; only the arrow highlights on hover.
- **Form:** plot size, facing (N/E/S/W compass picker, "road side"), floors (optional), services, name, town (optional) → opens an SMS to +91 91500 09835 with the details written in, and shows the message with a Copy button (desktop fallback). A small blueprint beside the form draws the visitor's own plot to scale as they type, with the road on the side they picked. Calling = the header number and both numbers in the footer (kept off the form so a number never shows twice on one screen).
- Favicon / home-screen icon from the "AVR" lettering (no logo exists); og image (1200×630) of the hero plan.

## Assumptions I made
- **+91** on both numbers (location-based; brief flags it as unconfirmed).
- **SMS as the form's channel.** Their own words say "Contact Now" by phone; texting isn't confirmed, so calling both numbers sits right under the send button. WhatsApp deliberately not used (brief: don't assume).
- **91500 09835 is the primary number** (it's the one the ad repeats in "Contact :"). 89259 78473 is in the form fallback and footer.
- **"We" voice** — the ad says "We Are Providing...".
- **Colors** (blueprint navy + marigold) are mine; there's no logo or brand color.
- **How it works** steps (plot → 2D Vastu plan → add 3D/approval/drawings) are inferred from the service list, not stated by them.
- The sample plan is illustrative, not one of their drawings. Room placements follow common Vastu practice.
- "Walkthrough video" shows "Ask us" — no price published.
- Spelling kept as they write it: "Vasthu" in the name, "Vastu" in "2D Vastu Plan".

## Placeholders and gaps
- No logo, no photos of their plans/3D renders, no reviews, no email, no Facebook business page (the only FB link is a post in a NJ contractors group — not linked, it would confuse customers in Tamil Nadu). So: no proof/work section and no Facebook link yet.
- Owner name, hours, years in business, base town (Tirunelveli vs Chennai) unknown.
- Footer has no email (none exists).

## Questions for the owner
- Do both numbers take SMS? WhatsApp? (WhatsApp would likely be the better form channel in India.)
- Can you send 6–10 of your 2D plans, 3D elevations and interiors renders? (These would become the work section, and the biggest upgrade.)
- A logo, if any. Owner's name (for "I'm ___" voice and trust).
- Which town is the base? Do you work only in Tirunelveli and Chennai, or anywhere in Tamil Nadu / online?
- Walkthrough video price. Price for floors above ground / plots over 1000 sq ft?
- Hours / best time to call.
- Should the site also be in Tamil?

## Ideas not built (yours to pick)
- **Runner-up world:** kolam — rice-flour lines drawn on a dark threshold, the finger draws kolam dots/loops. Warmer and more Tamil, less "architect".
- WhatsApp hand-off once confirmed (`https://wa.me/91...?text=`).
- Work gallery of their 3D elevations once supplied, framed as drawing sheets with a title block; Facebook link under it once they have a page.
- Tamil/English toggle.
- Facing picker that redraws the hero plan for the chosen direction (east/west/north/south-facing Vastu layouts).
- Document upload for "Online Approval Plan" (needs a backend; Muse suggested it as the hook).

## Impeccable pass (every mode except live)
Finish reviewer + critique, audit, harden, optimize, adapt, clarify, polish, layout, typeset, colorize, bolder, quieter, distill, animate, delight, overdrive. Applied: 360px header collision, landscape-phone scroll trap (plan height capped by `svh`), focus ring/field border contrast, checked-chip hover outline, accessible errors (`aria-invalid`/`aria-describedby`), compass radio order, text inputs instead of `type=number`, faster pen (60 ft/s, 9 s hold, opens on the finished outer walls), bigger canvas labels with the grid cleared behind them, drawn walls keep their length label, bigger price figures, sticky headings on desktop, plot preview (overdrive), duplicate phone line removed.
Rejected as against your rules: hero Call button / sticky bar, web fonts, WhatsApp, row hover tint, letting vertical swipes scroll the plan.
Detector findings left standing on purpose: `cream-palette` (drafting paper is the world), `flat-type-hierarchy` (counts only small UI sizes; display headings are clamp()), `cramped-padding` ×2 (hero plan bleeds to the section edge; price list top rule). `overused-font roboto` ignored in `.impeccable/config.json` (system stack is house style).
Process note: the direction was chosen unattended without a concept-roll seed.

## Not verified
- Real-device touch (iOS Safari, Android Chrome, Facebook in-app browser) — tested only with simulated pointer events in headless Chrome.
- The SMS hand-off on real phones, and whether Indian carriers/phones handle the `sms:+91…?&body=` link.
- Frame rate on low-end Android phones (likely the norm for this audience).
