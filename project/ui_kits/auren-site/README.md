# AUREN site — UI kit

A clickable, near-pixel recreation of the AUREN landing page per the brief in the root `README.md`.

## Files
- `index.html` — full page: nav, hero, about, how it works, directions, cases (masonry), for designers, testimonials, CTA, footer.
- `site.css` — page-level styles (tokens come from `../../colors_and_type.css`).

## Sections
1. Floating glass nav (pill, backdrop-blur)
2. Hero — `AUREN` + sparkle, "Studio of visual renewal", "14 days to new", two CTAs, ambient glow blobs + grain
3. About — copy + 4-tile pillar grid
4. How it works — 4-step timeline with dot markers
5. Directions — 12-tile invert-on-hover grid
6. Cases — masonry (3-col), hover meta panel, click → fullscreen lightbox
7. For designers — dark editorial block: "Not a freelance marketplace. A creative system." + perks + roster chips
8. Testimonials — 3-card row, one featured
9. CTA — "Your brand can look different in 14 days." + Start a project
10. Footer — dark, brand block + 3 link columns

## Interactions
- **Custom cursor** with `orbit / view / cta / text` variants, 18% lerp follow.
- **Scroll reveal** on every `.reveal` element via IntersectionObserver (blur → sharp).
- **Lightbox** for cases (click → fullscreen, ESC / click bg to close).
- **Filter chips** (cosmetic active state — no real filtering yet).
- All hover states use lime glow + lift.

## Substitution flags
- Days One is a free Google Font, used as the brief-specified display face. The wordmark in `auren-lockup.png` is a custom didone (lockup-only).
- Lucide icons aren't needed in the landing — every "icon" is the brand sparkle, an arrow glyph, or numerals.
