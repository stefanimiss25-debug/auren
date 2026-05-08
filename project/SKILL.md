---
name: auren-design
description: Use this skill to generate well-branded interfaces and assets for AUREN — a curated online design studio (Studio of Visual Renewal · 14 days to new) — either for production or throwaway prototypes/mocks/etc. Contains essential design guidelines, colors, type, fonts, assets, and UI kit components for prototyping.
user-invocable: true
---

Read the `README.md` file within this skill, and explore the other available files. Key files:

- `README.md` — brand context, sources, content fundamentals, visual foundations, iconography
- `colors_and_type.css` — every design token (colors, type, spacing, motion, shadows, glows, grain)
- `assets/` — logo mark + lockup, real case imagery (LUMEN FEST, СЕНОРА, posters, logos, AI visuals)
- `preview/*.html` — small specimen cards: type / color / spacing / components / brand
- `ui_kits/auren-site/` — clickable HTML recreation of the AUREN landing page

If creating visual artifacts (slides, mocks, throwaway prototypes, etc.), copy assets out and create static HTML files for the user to view, linking `colors_and_type.css` and the logo SVG. If working on production code, you can copy assets and read the rules to become an expert in designing with this brand.

If the user invokes this skill without any other guidance, ask them what they want to build or design, ask some questions, and act as an expert designer who outputs HTML artifacts _or_ production code, depending on the need.

## Quick rules of thumb
- **Voice:** calm, certain, fragmenty. RU-primary, EN editorial accents in ALL CAPS. No emoji. No exclamation points.
- **Type:** Days One (display) + Inter (body) + JetBrains Mono (technical). Tight tracking on display, wide on eyebrows.
- **Color:** milk + ink carry 90%. Lime is earned (numerals, glow, one CTA per screen). Lavender is ambient (glass, blobs, underline).
- **Layout:** lots of air. Pinterest × Behance masonry for cases. 144px section gaps.
- **Motion:** soft, slow, never bouncy except for floating objects. Reveal = blur → sharp.
- **Cursor:** custom required. Orbit by default, "View" over case images, lime fill over CTAs.
- **Icons:** Lucide for utility, brand sparkle for accent. Never emoji.
