# Operator sheet - tuans-dk-auto-repair

**Tier:** standard ($1000) - **Booking:** REQUIRED
**Business:** Tuan's DK Auto Repair | **Phone:** (714) 705-5957
**City:** Westminster CA | **Niche:** auto repair

## Evidence (use in OD - do not invent)

### Google Maps (this business)
- [Open Maps listing](https://www.google.com/maps/place/Tuan's+Dk+Auto+Repair/@33.7431719,-117.9722528,17z/data=!3m1!4b1!4m6!3m5!1s0x80dd27b51d9c2b39:0x3db482d2920f47ce!8m2!3d33.7431675!4d-117.9696779!16s%2Fg%2F1vxcwqnt?entry=ttu)
- Scrape notes: intake-from-link

### Review language (harvested - copy tone only)
1. "I was pleased with his quote and pleased that he uses ORIGINAL Dealer parts, which is important to me as well."
2. "I had a wonderful experience at Tuan's Dk Auto Repair. The owner is extremely helpful and truly dedicated to providing great service."
3. "Finally I stumbled across Tuans on Yelp. He had a solid 5 star which was reassuring. Tuan was very nice on the phone and told me to come by and he will see what he can do."

### Peer refs (layout research)
- [https://www.carrier.com/residential/en/us/](https://www.carrier.com/residential/en/us/) - Trust badges + emergency CTA hierarchy
- [https://www.lennox.com/residential/](https://www.lennox.com/residential/) - Service-area clarity, licensed contractor tone
- [https://www.trane.com/residential/](https://www.trane.com/residential/) - Seasonal offer blocks without slop gradients
- [https://styles.refero.design/category/home-services](https://styles.refero.design/category/home-services) - Refero trades pattern lock
- [https://www.google.com/maps/place/Tuan's+Dk+Auto+Repair/@33.7431719,-117.9722528,17z/data=!3m1!4b1!4m6!3m5!1s0x80dd27b51d9c2b39:0x3db482d2920f47ce!8m2!3d33.7431675!4d-117.9696779!16s%2Fg%2F1vxcwqnt?entry=ttu](https://www.google.com/maps/place/Tuan's+Dk+Auto+Repair/@33.7431719,-117.9722528,17z/data=!3m1!4b1!4m6!3m5!1s0x80dd27b51d9c2b39:0x3db482d2920f47ce!8m2!3d33.7431675!4d-117.9696779!16s%2Fg%2F1vxcwqnt?entry=ttu) - peer reference
- [https://www.carrier.com/residential/en/us/](https://www.carrier.com/residential/en/us/) - peer reference

## Creative angle
auto repair in Westminster, CA.
Commissioned local brand - distinctive typography and color, not a swapped template.
Local customers; primary CTA tap-to-call (714) 705-5957.

## Starter DNA
- Starter path: tools/od-starters/generic-local - open README before Pass 1

## Design DNA (never a template - your OD seed)
- **OD seed:** `workwear handcut ledger wordmark soft numerals brick`
- Full direction + forbidden list: `.rf/design-dna.md`. Reroll: `.\scripts\new-design-dna.ps1 -Slug tuans-dk-auto-repair -Force`

## Money systems (pitch these FIRST - the site second)
- **Foundation (bundled FREE in System tier):** Business Brain (`modules/crm/`) + Owner's
  Control Room (`modules/dashboard/`). One sheet, one login - every system below plugs into it.
- **START: Ghost Lead Catcher** `tools/rf-kit/modules/ghost-lead-catcher/` (+$400) - this niche's sharpest pain. LEAD with it on the call.
- Next sell 2: **Review Magnet** `modules/review-magnet/` (+$500) - near-zero wiring cost once the Brain is in.
- Next sell 3: **Come-Back Machine** `modules/retention/` (+$500) - near-zero wiring cost once the Brain is in.
- Next sell 4: **Thank-a-Friend Referral Tracker** `modules/referral-tracker/` (+$300) - near-zero wiring cost once the Brain is in.
- Return-visit motion: come back in 60-90 days and sell the next system on the path - the
  foundation is already installed, so margin RISES with each one.
- Suggested price-add over tier floor (modules + starting system): **+$400**. Stack with rubric (busy/reviews/rush).
- Full path lifetime value on this client: +$1700 across return visits.
- **Command Pack (install footprint day one):** Ghost Lead Catcher + Review Magnet + Come-Back Machine = list $1400, **bundled $1260** (save $140). More systems installed now = a richer Path C later.
- **Attach Monthly Wins Report** (+$300, or bundle it FREE on a System build): the monthly proof email is what turns this client into referrals and repeat sales.
- Brand Kit add-on: +$350 (new-brand-kit.ps1).
- Doctrine: pitch the money system first (caught leads, filled slots, reviews), the site second.
- Full spec (modules, placeholders, client setup): `.rf/system-spec.md`

## Showroom inventory (fork candidates)
- None yet for this niche. Unsold builds land here via `.\scripts\mark-unsold.ps1 -Slug <slug>`.

## Pricing (per-deal - never below floor, SOUL sec.3)
- Tier floor: $1000. Anchor high (pitch Website System first), sell down.
- Charge UP for: 100+ reviews/busy, money-moment module, multi-location/menu-heavy, rush.
- Brand Kit add-on: $350+. Log OD minutes at sale: `log-sale.ps1 -DesignMinutes <n>`.

## Booking snippet (Standard / Premium)
- RECOMMENDED: Templates/od-snippets/booking/request-form-formspree.html - Standard default - callback form unless owner prefers calendar | Alternate: Templates/od-snippets/booking/calendly-embed.html
- Replace placeholder **FORM_ID** with client endpoint before handback
- Checklist: `Templates/od-snippets/booking/checklist.md`
- After handback: `.\scripts\qa-standard-ship-bar.ps1 -Slug $Slug`

## Pass 1 - commission (~8 min, structure only)
```powershell
.\scripts\run-od-commission.ps1 -Slug tuans-dk-auto-repair
```

## Pass 2 - polish + mark (~9 min)
- [ ] Hero + phone above fold
- [ ] Callback form pasted from `Templates/od-snippets/booking/request-form-formspree.html` (trades)
- [ ] Placeholder `FORM_ID` replaced (client account)
- [ ] Greeter copy sounds like staff, not generic AI form
- [ ] Proof from Evidence section (no invented reviews)
```powershell
.\scripts\run-od-mark-design-ready.ps1 -Slug tuans-dk-auto-repair
```

## Handback (Grok)
```powershell
.\scripts\run-od-handback.ps1 -Slug tuans-dk-auto-repair -Package -Deploy
```