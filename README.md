# Mother Knows Best — The Conscious Style & Capsule Edit

> **Live App:** [https://rapid-prototyping-4134c--mum-style-compass-lsvhvb3c.web.app](https://rapid-prototyping-4134c--mum-style-compass-lsvhvb3c.web.app)
> **Community:** [https://motherknowsbest.ie](https://motherknowsbest.ie) — Greystones & Wicklow mums: toy swaps, monthly book club, support groups, local news.

A bright, retail-editorial **conscious wardrobe & body-confidence stylist** for mothers aged 25–45, built as the female counterpart to the men's [`style-savvy-pro`](https://github.com/Redser06/style-savvy-pro) (`StyleMate`) app.

The premise: when your body has changed, your mornings are chaos, and 90% of your money goes on the children, **you cannot afford wardrobe mistakes.** This app takes a mum from *"I have nothing to wear and I'm terrified of buying the wrong thing"* to a Jev-verified capsule of 3 bridge pieces that unlock 18+ outfits she already owns.

---

## The 4-Step Journey

| Step | Tab | What happens |
|---|---|---|
| **1** | `My Mum Stage` | She **self-identifies her personal circumstances** (Maternity Leave, Working Mum, Stay-at-Home, Returning to Work, WFH, Expecting) and sets her spend limit, body-confidence focus, and practicality gates. |
| **2** | `Stylist & Jev Interview` | A **conversational consultation with Maeve** (1-tap quick replies or free-text natural language) where the LLM + **TypeSafe AI `Jev` (`typesafe/jev-latest`)** parse her silhouette, seasonal skin undertone, and calibrated confidence in real time. |
| **3** | `Snap My Wardrobe (CV)` | She **photographs the pieces she already owns**. A live **HTML5 Canvas Computer Vision** pipeline extracts dominant hex colour, classifies warm/cool undertone, draws a CV bounding box, and maps each piece to Tab 4. |
| **4** | `★ The Conscious Edit (HERO)` | The **hero feature**: Part 01 = complete flattering outfit formulas (2 owned pieces + 1 bridge piece). Part 02 = Jev-scored capsule gap pieces with Cost-Per-Wear and Outfits Unlocked. |

Every step carries a **`⚡ Fast-Track to My Conscious Edit (Hero)`** shortcut so a busy mum can reach the payoff in one click.

---

## Why It's Purpose-Built for Mums (vs. the men's `style-savvy-pro`)

1. **Self-identification first.** The men's version drops you straight into a style quiz. This one starts with *"where are you in your motherhood journey right now?"* because a woman on maternity leave and a woman returning to a Dublin office need completely different cuts, fabrics, and budgets.
2. **Zero body-shame, zero measurements.** No tape measures, no weight, no dress size. Everything is framed around **proportion, drape, comfort, and fabric behaviour**.
3. **Postpartum & feeding reality is a first-class spec.** Nursing access, C-section-safe waistbands, 30°C machine wash, squat-proof stretch, and crease-free commute are hard filters, not nice-to-haves.
4. **Conscious mum math.** Every single recommendation shows **Cost-Per-Wear** and **New Outfits Unlocked** before any price, because the real budget constraint is family money, not personal income.
5. **TypeSafe AI `Jev` calibrated decisioning.** Each purchase is scored on a calibrated confidence level and a **buyer regret risk** percentage, so the app can honestly say *"only buy if it unlocks 4+ outfits."*
6. **The Mother Knows Best design system.** Warm Alabaster canvas, MKB Vermilion Red-Orange, MKB Soft Orchid Pink, and Deep Charcoal pill CTAs — lifted directly from the `motherknowsbest.ie` community identity, with editorial retail photography throughout.

---

## The Design System (`DESIGN.md`)

A formal [Google `DESIGN.md`](https://github.com/google-labs/design.md) token spec, lint-verified with **0 errors and 0 warnings**:

```bash
npx -y @google/design.md lint DESIGN.md
```

| Token | Value | Role |
|---|---|---|
| `primary` | `#C82D08` | MKB Vermilion Red-Orange (WCAG-AA `5.51:1` on white) |
| `secondary` | `#1F2022` | Deep Charcoal pill CTAs |
| `tertiary` | `#006948` | Coastal Sage — Jev confidence + Cost-Per-Wear |
| `neutral` | `#F9F8F4` | Warm Alabaster page canvas |
| `mkb-pink` / `mkb-light-pink` | `#FBCFFA` / `#FEEAFD` | MKB Orchid Pink community accents |
| Type | `Newsreader` (editorial serif, italic accents) + `Plus Jakarta Sans` + `JetBrains Mono` (telemetry) | |

---

## Run in one command

```bash
cd mum-style-studio && python3 -m http.server 8899
```

Then open:
- **Direct App URL:** http://localhost:8899/
- **Deep-Link Views:**
  - `http://localhost:8899/?tab=journey` — 1. Self-Identify Mum Stage
  - `http://localhost:8899/?tab=interview` — 2. Stylist & Jev Interview
  - `http://localhost:8899/?tab=wardrobe` — 3. Snap My Wardrobe (CV)
  - `http://localhost:8899/?tab=shop` — 4. ★ The Conscious Edit (HERO)

No build step, no `npm install`, no toolchain. It's a PWA: open in a browser and use **Add to Home Screen** (iOS Safari) or **Install** (Android Chrome).

---

## Tech Notes

- **Stack:** single-file HTML + vanilla JS + Tailwind (CDN) + `Newsreader`/`Plus Jakarta Sans`/`JetBrains Mono` (Google Fonts). Zero dependencies to install.
- **PWA:** `manifest.json` + `sw.js` for installability and offline shell caching.
- **Computer Vision:** real HTML5 `<canvas>` pixel sampling (dominant hex extraction, warm/cool undertone classification) — runs entirely client-side, so **no photo ever leaves the device**.
- **LLM bridge:** optional Gemini API key (`gemini-3.8-flash` for fast parsing, `gemini-4-argon` for heavy reasoning) for the free-text stylist interview. Falls back to a deterministic on-device stylist engine when no key is present.
- **Jev engine:** a local calibrated evaluator mirroring the `typesafe/jev-latest` schema (Silhouette Flatter Level `1–5`, Calibrated Confidence, Regret Probability, Budget & Practicality Hurdle Penalties) so the prototype runs with zero network dependency.
- **Privacy:** 100% anonymous. No accounts, no measurements, no photo storage.

---

## Roadmap

1. **Mother Knows Best pre-loved swap feed** — source Tab 4 bridge items from the `motherknowsbest.ie` Greystones/Wicklow Buy & Sell board before buying new.
2. **Multi-garment rail segmentation** — one photo of a whole wardrobe rail auto-segments into 5–8 tagged garments via Gemini Vision.
3. **7:15 AM school-run weather push** — Met Éireann morning forecast + her photographed wardrobe → one zero-decision outfit formula.

---

## Credits

Built by [Conor Redmond](https://github.com/Redser06) with the Hermes agent fleet.
Community identity & colour system from **Mother Knows Best Wicklow** ([motherknowsbest.ie](https://motherknowsbest.ie)).
