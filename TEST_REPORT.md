# TEST REPORT — Manjunath Electricals
> Date: 2026-09-10 | Tester: Senior Engg | Segment: Retail/Service (Tier-2)

## Build
- [x] `npm run build` PASS (vite 5.4.21, 4 modules, 0 warnings)
- dist sizes: 14.32 kB HTML / 12.13 kB CSS / 1.20 kB JS (dist total ~36K) — well under perf budget

## Static checks (all PASS)
- [x] NO tel:/wa.me/phone anywhere (CSV phone empty — never invented); Directions/Maps CTAs only
- [x] data-missing flag: `<!-- data-missing: phone -->` + visible "Phone not listed" notes (hero, services note, visit)
- [x] Google Maps URL present (nav, hero, reviews, visit, mobile Directions button)
- [x] JSON-LD Electrician schema, no telephone, rating 5.0, hasMap
- [x] Tipu Sultan Circle / near State Bank landmark in hero, address, FAQ; H1, semantic sections, skip link, async fonts
- [x] Retail pilot copy adapted to services (wiring, lighting/fans, appliances, repair enquiries), contrast-safe indigo/gold
- [x] No lorem ipsum, no invented products/charges/hours (in-store confirmation fallback)
- [x] aria-expanded on nav toggle; base '/sindagi-manjunath-electricals/'; favicon in dist

## Pending (requires preview + device lab before Deployed)
- [ ] Lighthouse CI mobile+desktop (target 90/95/95/95)
- [ ] Playwright E2E + axe (0 serious) + linkinator
- [ ] Screenshots 360/768/1440
- [ ] GitHub Pages deploy verify (200 + base path assets)

## Verdict: BUILT + STATIC QA PASS → ready for full QA + separate repo deploy
