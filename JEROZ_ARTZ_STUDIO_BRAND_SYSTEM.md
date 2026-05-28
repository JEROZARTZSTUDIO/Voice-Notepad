# JEROZ ARTZ STUDIO — Visual System

## 1) Brand Direction

**Positioning:** A premium art studio identity that feels editorial, collectible, and modern.  
**Design intent:** High-contrast, typography-led layouts with deliberate negative space and curatorial rhythm.  
**Tone:** Assertive, intelligent, refined, and cultural.

### Core Principles
1. **Contrast as confidence** — Use hard black/ivory contrast as the base; color appears as a controlled accent.
2. **Typography is the image** — Headlines carry emotional weight before photography does.
3. **Structured hierarchy** — Every composition should read in three scans: headline, context, action.
4. **Intentional spacing** — White space is not empty; it frames meaning and increases perceived value.
5. **Curated restraint** — Fewer elements, stronger decisions.

---

## 2) Color System (High-Contrast Editorial)

### Primary Palette
- **Obsidian** `#0A0A0A` — Core text/background anchor.
- **Ivory Paper** `#F6F2EA` — Primary light background.
- **Gallery White** `#FFFCF7` — Alternate light panel background.

### Accent Palette (Brand-Specific)
- **Carmine Ink** `#9E1B32` — Signature accent for links, tags, and selective highlights.
- **Gold Leaf** `#B08A3C` — Premium metadata accent and fine lines.
- **Electric Cobalt** `#2D4BFF` — Rare digital accent for interactive states.

### Neutral Ramp
- **Charcoal 800** `#1B1B1B`
- **Slate 600** `#4B4B4B`
- **Stone 400** `#8E8A84`
- **Mist 200** `#D8D2C7`

### Color Usage Ratios
- 70% light base (`Ivory Paper` / `Gallery White`)
- 20% dark structure (`Obsidian` / `Charcoal`)
- 10% accent (`Carmine Ink` + `Gold Leaf`, with Cobalt reserved for interaction only)

---

## 3) Typography System

### Typeface Pairing
- **Display Serif (Headlines):** `Canela` (fallback: `"Noe Display", "Times New Roman", serif`)
- **Editorial Sans (UI + Body):** `Söhne` (fallback: `"Inter", "Helvetica Neue", Arial, sans-serif`)
- **Mono (Metadata):** `IBM Plex Mono` (fallback: `"SFMono-Regular", Consolas, monospace`)

### Type Scale
- **H1 / Manifesto:** 80/76, tracking -0.02em, weight 500
- **H2 / Feature Title:** 56/56, tracking -0.015em, weight 500
- **H3 / Section Title:** 36/40, tracking -0.01em, weight 500
- **Lead Paragraph:** 24/36, tracking 0, weight 400
- **Body:** 18/30, tracking 0.002em, weight 400
- **Caption / Meta:** 12/18, tracking 0.08em, weight 500, uppercase

### Typographic Rules
- Use serif only for display tiers (H1–H3).
- Keep body copy sans-serif for clarity and modernity.
- Limit line length to **60–75 characters** for editorial reading comfort.
- Use uppercase mono for category labels, dates, and edition markers.

---

## 4) Layout and Spatial Hierarchy

### Grid
- **Desktop:** 12-column grid, 80px outer margins, 24px gutters.
- **Tablet:** 8-column grid, 40px margins, 20px gutters.
- **Mobile:** 4-column grid, 20px margins, 16px gutters.

### Spacing Scale (8pt Base)
`8, 16, 24, 32, 48, 64, 96, 128`

### Section Rhythm
- Hero top padding: **128px** desktop / **80px** mobile.
- Section padding: **96px** desktop / **64px** mobile.
- Card internal padding: **32px**.
- Copy block spacing: **24px** between heading and paragraph; **16px** between paragraphs.

### Hierarchy Pattern
1. **Primary Statement** (large serif headline)
2. **Contextual Narrative** (lead paragraph + metadata)
3. **Action Layer** (link/button with directional cue)

---

## 5) Components (Editorial-First)

### Hero
- Full-bleed neutral background.
- Massive headline (max two lines).
- Thin gold divider line beneath title.
- Meta row in mono uppercase.

### Feature Card
- Image or color field at top.
- Title (serif), short dek (sans), category/date (mono).
- Hover: 2px Carmine underline expansion + subtle upward translate (2px).

### Navigation
- Minimal top nav with generous spacing.
- Active state: Carmine text with 1px Gold underline offset.
- Avoid filled nav pills; prioritize typographic states.

### Buttons
- **Primary:** Obsidian background, Ivory text, square corners.
- **Secondary:** Transparent with Obsidian 1px stroke.
- **Micro-interaction:** 120ms color transition, 160ms transform.

---

## 6) Imagery & Art Direction

- Prefer monochrome or desaturated photography with one accent color introduced through styling.
- Use close crops, textured surfaces, studio details, and archival framing.
- Avoid generic stock aesthetics (smiling teams, flat-lay clichés, random gradients).
- Pair images with strong captions and edition context to reinforce curatorial voice.

---

## 7) Motion Behavior

- Motion should feel **editorial and deliberate**, never playful.
- Use reveal transitions that follow reading direction (bottom-to-top or left-to-right).
- Recommended durations:
  - 120ms: hover affordances
  - 240ms: card entrances
  - 400ms: section reveals
- Use `ease-out` or custom cubic-bezier `(0.22, 1, 0.36, 1)`.

---

## 8) Voice in UI Copy

- Prefer concise, curatorial language:
  - “Current Exhibition” instead of “Latest Work”
  - “View Catalogue” instead of “See More”
  - “Request Private Viewing” instead of “Contact Us”

- Sentence case for body text; uppercase only for metadata labels.

---

## 9) Accessibility & Legibility

- Maintain WCAG contrast of at least 4.5:1 for body text.
- Never place Carmine text on dark backgrounds without sufficient luminance support.
- Minimum body text size: 16px.
- Focus states must be visible with a 2px Cobalt outline.

---

## 10) Implementation Tokens

Use the companion token file:
- `jeroz-artz-tokens.css`

This token layer encodes color, type, spacing, motion, and component baselines for consistent rollout.
