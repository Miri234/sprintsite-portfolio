# SprintSite · UI/UX Pro Max design system
Updated: 2026-11-14

## Purpose
A conversion-focused showcase for small businesses in Azerbaijan. The three static HTML pages remain clearly labeled demos. No fake customers, reviews or sales figures.

## Source
Open-source [UI UX Pro Max](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill) (MIT). Project-local skill: `.agents/skills/ui-ux-pro-max/SKILL.md`.

Run (Python 3): `python .agents/skills/ui-ux-pro-max/scripts/search.py "portfolio agency minimal" --design-system -p SprintSite`.

The skill's dataset was consulted for:
- Portfolio/Personal: neutral background, restrained accent, clear project grid and contact CTA.
- Automotive/Car Dealership: premium dark/metallic, bold statement typography, energetic action accent.
- Bakery/Cafe: warm cream/brown, readable editorial type and menu-focused navigation.
- UX: 44×44 minimum interactive targets; visible keyboard focus; mobile reflow; contrast; reduced-motion support; no fake performance claims.

## 1. Portfolio — SprintSite
- Pattern: Hero → Projects → Pricing → Process → WhatsApp CTA.
- Style: contemporary minimal / Swiss-inspired; no misleading testimonials.
- Primary accent: `#315BF1`; ink `#152036`; background `#F6F7F8`; white cards.
- Display: Space Grotesk; body: DM Sans (with system fallbacks).
- WhatsApp prefill: `wa.me/994705337722`.
- File: `index.html`.

## 2. Automotive — VELOCE
- Pattern: Editorial hero → 3 details → services → demo booking/CTA.
- Style: premium dark motorsport with expressive type.
- Accent `#FF755F`; background `#0A0D13`; contrast text `#F7F5F1`.
- Display: Barlow Condensed; body: Manrope.
- Demo booking buttons deliberately trigger an informational toast: the fictional business does not take real reservations.
- File: `demos/auto.html`.

## 3. Cafe — MOKKA
- Pattern: Editorial hero → menu filters → menu cards → demo CTA.
- Style: warm editorial café, serif headline, friendly touch targets.
- Ink `#32261D`; brown `#75472D`; cream `#FCF8F1`.
- Display: Fraunces; body: DM Sans.
- Menu filter JS is preserved; mock order buttons deliberately show a demo notice.
- File: `demos/cafe.html`.

## UX acceptance checklist
- [x] No promises of actual customers/reviews; demo disclaimers remain prominent.
- [x] Main site sales CTA leads to WhatsApp.
- [x] Responsive layout breakpoints for mobile/tablet/desktop.
- [x] Keyboard focus-visible CSS and reduced motion fallback.
- [x] Mobile menu filtering kept functional.
- [x] Cross-page WhatsApp number preserved.
- [ ] Lighthouse automated scoring / full WCAG audit — not performed.

## Change strategy
Edit the existing HTML, preserve meaningful business behavior, re-test all three public routes, and avoid exposing API keys or introducing paid hosting dependencies.
