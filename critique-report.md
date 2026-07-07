# Critique Report (impeccable + ReviveForge enforced pass)

**Reviewer:** ReviveForge impeccable/taste structured critique (pre-gate enforced)
**Verdict:** Fix before ship

## Taste dials in effect
- DESIGN_VARIANCE: medium-high
- MOTION_INTENSITY: cinematic
- VISUAL_DENSITY: medium

## Keep
- Intake-grounded NAP and persona copy: exact phone (714) 705-5957, address, harvested reviews from BRIEF/PRODUCT
- Evidence-bound service descriptions and proof facts tied to real reviews
- Cinematic stagger animations + reduced-motion handling
- Mobile-first tap-to-call CTAs and after-hours form swap

## Fix
- Missing DESIGN-AESTHETIC.md: DESIGN.md sparse (typography + dials only); lacks accent, visual rules, self-hosted font paths, component specs per DESIGN-BRIEF and PRODUCT anti-references
- Hero visual anchor weak: pure dark CSS band with headline, fact box, sub, CTAs. No photo, illustration, or cinematic graphic to ground viewport; radials lack contrast/hierarchy
- Card grids violate anti-slop: .svc-item and .quote-card create multiple bordered hover cards (services grid, reviews 2-col span); nested visual noise. Figtree sans approximates Inter defaults
- Typography breach: Google CDN Fraunces/Figtree preload instead of self-hosted premium fonts per PRODUCT + DESIGN
- Proof uses heavy inline <style> + grids; proof-aside reads as nested card, breaking hierarchy
- Header phone links masked (+171****5957) vs full BRIEF/meta number

## Quick wins
- Add DESIGN-AESTHETIC.md: self-hosted fonts, accent, no-card rule, hero visual spec, hierarchy/contrast
- Anchor hero with photo treatment, bold mark, or high-contrast graphic for cinematic presence
- Flatten services/reviews to lists or single-contrast blocks; drop card borders/shadows
- Switch to self-hosted fonts; remove Google preconnects
- Re-run impeccable critique; clear all Fix items pre-pipeline (Test-RFCritiquePass blocks on unresolved)