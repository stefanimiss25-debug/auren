# AUREN Design System

> **AUREN — Studio of Visual Renewal · 14 days to new.**
> Online curated design studio. Not a freelance marketplace — a creative system.

AUREN is a digital‑native design studio + curated platform: a client describes the job, AUREN matches them with a designer from the roster, and a finished project ships in 14 days. The roster spans brand identity, web, UX/UI, motion, AI visuals, packaging, SMM design, content, 3D, presentations, video editing, and creative direction.

This repo is the brand & UI design system: tokens, typography, brand assets, copy guidelines, and a clickable UI kit recreating the AUREN site itself.

---

## Sources & inputs

This system was assembled from:

- **Logo & wordmark** — uploaded files
  - `assets/auren-mark.png` (4‑pointed sparkle, lavender body, lime spark, black ring)
  - `assets/auren-lockup.png` (full wordmark: AUREN · STUDIO OF VISUAL RENEWAL · 14 DAYS TO NEW)
  - `assets/auren-mark.svg` (vector recreation for in‑product use)
- **Brief** — pasted text from the user (May 2026): full site spec covering hero / about / how‑it‑works / directions / cases / for designers / reviews / CTA / footer, plus type, color, motion, and inspiration list.
- **Founder portfolio** — [`stefanimiss25-debug/stefania-portfolio`](https://github.com/stefanimiss25-debug/stefania-portfolio) (public). Source of real case imagery (LUMEN FEST, СЕНОРА, posters, logos, AI visuals). Imported into `assets/case-*.png`.
- **Empty repo** — [`stefanimiss25-debug/auren`](https://github.com/stefanimiss25-debug/auren) (the AUREN site repo, currently empty — this design system is the spec it should be built against).
- The mounted local `auren/` folder was empty at the time of build.

> Founder/designer of record: **Стефания** (Volgograd, RU). Email `stefanimiss07@gmail.com`, Telegram `@stefanimis`, IG `auren_design14`.

---

## Index

```
AUREN-design-system/
├── README.md                  ← you are here
├── SKILL.md                   ← Agent Skills entry point
├── colors_and_type.css        ← all design tokens (colors, type, spacing, motion)
├── assets/
│   ├── auren-mark.png|.svg    ← logo mark (sparkle)
│   ├── auren-lockup.png       ← full wordmark
│   ├── case-lumen-*.png       ← Lumen Fest case imagery
│   ├── case-senora-*.png      ← СЕНОРА case imagery
│   ├── case-poster-*.png      ← posters
│   ├── case-logo-*.png        ← logos
│   └── case-ai-*.png          ← AI visuals
├── preview/                   ← design‑system tab cards (700×N each)
└── ui_kits/
    └── auren-site/            ← clickable recreation of the AUREN site
        ├── index.html         ← live demo of the full site
        ├── components.jsx     ← Header, Hero, Cases, Cards, etc.
        └── README.md
```

---

## CONTENT FUNDAMENTALS

### Voice

AUREN writes the way a strong young creative team talks: **calm, certain, emotionally precise**, never corporate. Russian is primary, English is woven in for fashion / digital‑gallery effect (the wordmark itself is bilingual: `AUREN · STUDIO OF VISUAL RENEWAL · 14 DAYS TO NEW`). The voice is closer to Acne Studios than Behance — **stating, not selling**.

- **First person** is rare. The studio mostly says "AUREN" or "мы / we".
- "**Ты**" is reserved for designer‑facing copy ("любой дизайнер может попасть в AUREN"). Client‑facing copy is neutral / "вы".
- **Sentence fragments are encouraged.** One‑breath statements arranged on the page like signage.
  > Дизайн через состояние. Не через шаблон.
  > Не «биржа фриланса», а curated online‑studio.
- **No emoji.** No exclamation points. No "✨" or "🚀" — the spark is the logo's job.
- **No hype words.** Avoid: revolution, game‑changing, ultimate, best, world‑class. Replace with concrete promises ("14 days to new").
- **English ALL CAPS** for editorial labels and CTA: `STUDIO OF VISUAL RENEWAL`, `START A PROJECT`, `JOIN AUREN`. Wide tracking (~0.22em).
- **Mixed‑language allowed.** "kidcore", "future medieval", "art‑дирекшн", "AI‑креатор" — keeps the editorial / fashion register.
- **Numerals are characters.** "14 days to new" — the 14 is literally accent‑coloured in the lockup. Treat numerals as design.

### Casing

| Surface | Casing |
|---|---|
| Display headlines (Days One) | Sentence case in RU; ALL CAPS in EN. |
| Section labels / eyebrows | `ALL CAPS · WIDE TRACKING` |
| Body copy | Sentence case |
| CTA buttons | `START A PROJECT` (en) / `Найти дизайнера` (ru) |
| Direction tags ("Brand Identity", "Motion") | Title Case |

### Examples (use as anchor)

- Hero (RU/EN bilingual): **"AUREN — STUDIO OF VISUAL RENEWAL"** / **"14 DAYS TO NEW"**
- Manifesto: **"NOT A FREELANCE MARKETPLACE. A CREATIVE SYSTEM."**
- Closing CTA: **"YOUR BRAND CAN LOOK DIFFERENT IN 14 DAYS."** → `START A PROJECT`
- Section eyebrow examples: `01 · ABOUT`, `КАК ЭТО РАБОТАЕТ`, `DIRECTIONS`, `SELECTED WORK`.
- Process step microcopy: "Оставляете заявку" / "Мы подбираем дизайнера" / "Утверждаете стиль и бюджет" / "Получаете результат за 14 дней".

---

## VISUAL FOUNDATIONS

### The system in one paragraph

Lots of air. Editorial, fashion‑adjacent. **Milk‑white** ground (`#F7F5F0`), **deep ink** (`#0A0A0B`), one pop of **acid lime** (`#D8FF3E`) and a soft **lavender** (`#C7B6DC`) — both straight from the logo. Type pairs **Days One** (chunky, fashion / digital aesthetic) for display with **Inter** for everything else. Layouts are masonry‑adjacent — Pinterest × Behance — with whitespace doing the heavy lifting. Movement is everywhere but never loud: floating 3D objects, slow ambient drift, hover glow, blur → sharp transitions. Inspiration sits between **Apple, Acne Studios, Awwwards, Behance, LINII, COSMOS** and modern fashion brands.

### Color

Two brand accents (lime + lavender) on a milk‑white / deep‑ink ground. Lime is **earned** — it shows up on numerals, hover glows, the spark, and one CTA per screen. Lavender is the soft "aura" — used on glass cards, ambient blobs, and underline accents. Neutrals carry 90% of the page. Defined as CSS variables in `colors_and_type.css` (`--auren-lime`, `--auren-lavender`, `--auren-milk`, `--auren-ink`, etc.).

### Type

- **Display: Days One** (Google Fonts, free) — chunky, single‑weight, slightly retro / fashion / digital. Used for the hero, case titles, manifesto pull‑quotes.
- **Body: Inter** — clean, neutral, gives Days One the contrast it needs.
- **Mono: JetBrains Mono** — captions, numerals, technical labels (`01 / 04`, `14 DAYS`).
- High contrast between very‑large display and small body. **No mid‑sizes.**
- Tight tracking on display (`-0.02em`), wide tracking on eyebrows (`+0.22em`).
- The original wordmark in `auren-lockup.png` uses a custom didone — that's lockup‑only. Days One is the working face.

> **Substitution flag:** Days One is the brief‑specified working face (free). The wordmark in the lockup PNG appears to be a **bespoke didone**. If a licensed display face exists for the brand (e.g. Editorial New, Reckless, Bodoni Moda), please share — we'll swap it in.

### Spacing & layout

- 8‑pt grid (`--auren-space-*`), with a deliberate 144px "lots of air" gap (`--auren-space-10`) between hero and the next section.
- Site grid: 12‑col, 1440px max, **wide gutters** (24–32px). Cases break out of the grid into masonry.
- Section padding: `space-9 → space-10` top/bottom on landing.

### Backgrounds

- **Default:** flat milk (`#F7F5F0`), no texture.
- **Dark variants** (footer, fullscreen preview, manifesto): deep ink with a **subtle film grain** (the `--auren-grain` SVG noise) and a slow lavender glow blob drifting in the background.
- **Hero:** milk + 1–2 ambient lavender / lime glow blobs, blurred ~80px, slow drift (~30–60s loop).
- **No gradient backgrounds as primary surface.** Glow blobs are scoped to layered overlays.
- Full‑bleed imagery only inside cases (the case art is the surface).

### Animation

- Hero text: stagger reveal (60ms between elements), `opacity 0 → 1`, `translateY(24px) → 0`, `filter: blur(8px) → blur(0)`. Easing: `cubic-bezier(0.2, 0.75, 0.2, 1)`. Duration ~900ms.
- Scroll reveal: same recipe, threshold ~0.18, `--auren-dur-3` (560ms).
- **No bounces** on UI. Springs (`--auren-ease-spring`) are reserved for floating 3D objects and the cursor.
- Case cards: idle "breathing" — `scale(1) ↔ scale(1.005)` on a 6–8s loop, off‑sync per card.
- Hover: lift 4–7px, soft shadow expand, image saturates +8%, spark‑lime border glow on primary CTAs.
- 3D / abstract objects in hero: continuous slow rotation + parallax tied to cursor.
- Reduced motion: all of the above → instant in‑view.

### Hover & press states

- **Buttons:** lift `translateY(-2px)`, glow `--auren-glow-lime`, slight letter‑spacing increase (+0.005em). Press → `translateY(0) scale(0.98)`.
- **Cards:** lift `-7px`, shadow `--auren-shadow-3`, image scales 1.015. No tint.
- **Links (text):** underline animates from 0 → 100% width, lavender deep colour.
- **Image cards (cases):** on hover, fullscreen preview affordance fades in (corner arrow + overlay caption); click → opens fullscreen lightbox.
- **Icons:** rotate spark icon 90° on hover.

### Borders & dividers

- Borders are **hairline** — `1px solid rgba(10,10,11,0.10)` on milk; `rgba(255,255,255,0.14)` on dark.
- Cases & cards prefer **no border**, just shadow + radius. Dividers are 1px hairlines, generously spaced (32–48px gutters).

### Shadows / elevation

- 4‑step shadow system: `--auren-shadow-1..4`. 1 = inputs, 2 = cards at rest, 3 = cards hovered, 4 = floating panels / fullscreen preview drop.
- **Plus glows:** `--auren-glow-lime` and `--auren-glow-lavender` for hover states and floating objects. Glows are **ambient** — large blur radius, low alpha — never harsh outer shadows.

### Glass / blur / transparency

- Used for the **floating top nav** (milk @ 55% + 24px blur), **case overlay captions** (dark glass), and **how‑it‑works cards** when they sit over imagery.
- `backdrop-filter: blur(20–28px)` + `1px` glass border (`--auren-glass-border`).
- **Transparency is never decorative.** It signals "this floats above content."

### Imagery vibe

- Case imagery is **warm‑neutral**, often grainy, with strong art direction. AI visuals run cooler / more atmospheric. Avoid generic stock — every image earns its place.
- Posters and identity work skew warm‑bordeaux / olive — they pair beautifully with lime as a secondary accent.

### Corner radii

- `--auren-r-1` 4px (chips, inputs)
- `--auren-r-2` 10px (small cards)
- `--auren-r-3` 16px (default card)
- `--auren-r-4` 24px (large feature cards)
- `--auren-r-5` 36px (hero glass panels)
- `--auren-r-pill` 999px (buttons, tags, eyebrow chips)

### Cards

- Default: `--auren-milk-2` ground, `--auren-r-3`, `--auren-shadow-2`, no border. Padding `space-5` to `space-6`.
- Glass variant: `--auren-glass-light` background, `--auren-glass-border` border, 24px backdrop blur.
- Case card: full‑bleed image, `--auren-r-3`, no padding around the image, caption sits below in flow.

### Cursor

Custom cursor required (per brief). Default style:

- **Outer ring:** 28px lavender circle, 1px stroke, low‑alpha fill.
- **Inner dot:** 6px lime, follows cursor with 8% lerp lag (the orbit feel).
- **Variants** by hover target:
  - Over case image → grows to 56px, label inside ("VIEW").
  - Over text → shrinks to thin vertical bar (text caret hint).
  - Over CTA → fills lime with ink ring.
- The **logo sparkle** itself can be used as a cursor on the hero only — purple star with green dot inside, scales on click.

---

## ICONOGRAPHY

AUREN uses **Lucide** (CDN) as its icon set — clean 1.5px stroke, geometric, neutral enough to disappear next to the chunky Days One display. Lucide is loaded from `https://unpkg.com/lucide@latest/dist/umd/lucide.js`.

- **Stroke width:** 1.5 (default). Stroke color always inherits from `currentColor`.
- **Sizes:** 16 / 20 / 24 / 32 — match body text x‑height or a 2x grid step.
- **No filled icons.** Stroke only.
- **No emoji** anywhere on the AUREN surface. The spark sigil replaces decorative emoji needs.
- **Unicode:** `→` arrows are used heavily as inline accents in body copy, lists, and "next" affordances. `·` (middle dot) separates eyebrow phrases (`14 DAYS · TO NEW`).
- **The brand sparkle** (`assets/auren-mark.svg`, also exported inline as a React component) is the **only proprietary icon**. It pulls double duty as: logomark, list bullet (small), CTA spark, cursor variant, loading state. Always uses lavender body + lime dot + black ring.
- **Custom SVGs:** discouraged for general icons. If a concept isn't in Lucide, request the asset rather than drawing one.

> **Substitution flag:** No bespoke icon library exists yet. Lucide is the closest CDN match (geometric, hairline). Once a custom icon library is needed, we'll add `assets/icons/*.svg`.

---

## How to use this design system

- **In a new design / mock**: link `colors_and_type.css` and use the variables. Pull logos from `assets/`.
- **In a slide / pitch**: the lockup is `assets/auren-lockup.png`; the mark is `assets/auren-mark.svg`. Type tokens are CSS but are easily mirrored in any design tool.
- **In a UI kit / production code**: see `ui_kits/auren-site/` for component patterns.
- **Under Claude Code**: read `SKILL.md` at the root of this directory.
