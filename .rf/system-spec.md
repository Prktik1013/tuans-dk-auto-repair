# System spec - Tuan's DK Auto Repair

Niche:   (bucket: misc)  |  Tier: standard

## Job to be done
Someone lands at 9pm and needs one clear next step. Paste the bricks below in Open Design;
fill the CLIENT_* placeholders before handback (test-rf-modules.ps1 enforces the swap).

## Recommended modules
- **Lead form (REQUIRED for the Brain):** `tools/rf-kit/modules/crm/sheet-connector.html` -
  the contact form on the page MUST be this one. It writes every lead into the Brain sheet AND
  emails the owner. The plain `booking/web3forms-request-form` is EMAIL-ONLY: if you ship that,
  the Brain stays empty and every money-system below has nothing to work on. The System ship bar
  FAILS a Brain build whose page does not write to the sheet.
- No add-on modules at this tier - booking only. Upsell later if the lead is busy.

## Business Brain path (start here, then compound)
- **Foundation (bundled FREE in System tier):** Business Brain (`modules/crm/`) + Owner's
  Control Room (`modules/dashboard/`). One sheet, one login - every system below plugs into it.
- **START: Ghost Lead Catcher** `tools/rf-kit/modules/ghost-lead-catcher/` (+$400) - this niche's sharpest pain. LEAD with it on the call.
- Next sell 2: **Review Magnet** `modules/review-magnet/` (+$500) - near-zero wiring cost once the Brain is in.
- Next sell 3: **Come-Back Machine** `modules/retention/` (+$500) - near-zero wiring cost once the Brain is in.
- Next sell 4: **Thank-a-Friend Referral Tracker** `modules/referral-tracker/` (+$300) - near-zero wiring cost once the Brain is in.
- Return-visit motion: come back in 60-90 days and sell the next system on the path - the
  foundation is already installed, so margin RISES with each one.

## Client setup needed
- Web3Forms access key (email-only, free 250/mo) - see modules/OWNERS-GUIDE.md
- Business Brain sheet + /exec URL (8 min, once) - see modules/crm/SETUP.md
- Ghost Lead Catcher: see modules/ghost-lead-catcher/SETUP.md (engines paste into the SAME Brain script)

## Pricing signal
- Suggested price-add over tier floor (modules + starting system): **+$400**. Stack with rubric (busy/reviews/rush).
- Full path lifetime value on this client: +$1700 across return visits.
- **Command Pack (install footprint day one):** Ghost Lead Catcher + Review Magnet + Come-Back Machine = list $1400, **bundled $1260** (save $140). More systems installed now = a richer Path C later.
- **Attach Monthly Wins Report** (+$300, or bundle it FREE on a System build): the monthly proof email is what turns this client into referrals and repeat sales.
- Brand Kit add-on: +$350 (new-brand-kit.ps1).
- Doctrine: pitch the money system first (caught leads, filled slots, reviews), the site second.
