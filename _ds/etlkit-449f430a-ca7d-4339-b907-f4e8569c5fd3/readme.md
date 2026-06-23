# EtlKit Design System

Brand foundations for **EtlKit** — a modern, open-source ETL (Extract · Transform · Load) toolkit. EtlKit is an independent fork that continues the spirit of a long-running open-source ETL project while shedding its old identity: the box is gone, and so is the word "box."

This is a **brand-only** system — icon, colour, type and spacing tokens, plus specimen cards. It deliberately ships no component library or UI kit; consuming projects bring their own UI and inherit the EtlKit look through `styles.css` and the brand assets.

> Not affiliated with, or branded as, RapidSoft. The aesthetic lineage is acknowledged, but EtlKit is its own project.

---

## THE MARK — "Ascending Flow"

Three nodes — **Extract → Transform → Load** — riding a single confident curve upward and out of frame. It keeps the original project's heritage gesture (open, rising, energetic) without any container. The shape reads as data in motion and as a project that's open to development.

- **Primary mark:** `assets/logo/etlkit-mark.svg` (vermillion) · `etlkit-mark-ink.svg` · `etlkit-mark-white.svg`
- **Avatar / favicon:** `etlkit-avatar.svg` + PNGs (`etlkit-avatar-512/192`, `etlkit-favicon-32/16`) — a solid vermillion disc with the mark knocked out in white, so it survives down to 16px where a bare line would vanish.
- **Lockup:** `etlkit-lockup.svg` — mark + **Etl**Kit wordmark (Etl in ink, Kit in vermillion).

**Usage:** the bare mark on light surfaces; the disc for circular avatars and browser tabs. Don't recolour outside the vermillion/ink/white set, rotate, add effects, or enclose it in a box.

---

## VISUAL FOUNDATIONS

**Colour.** One decisive brand accent: **Vermillion `#F8462D`** — energy and openness against calm neutrals. A vermillion ramp (`50–700`) covers tints and states. Neutrals are a cool gray ramp on near-black ink `#16161A`; page background gray `#F5F5F7`, cards pure white. Feedback colours (success/warning/danger/info) are kept distinct from the brand red, with **Info** a trustworthy blue `#2A6FDB`. Use vermillion intentionally — a little against the gray goes a long way.

**Type.** **Space Grotesk** (Regular/Medium/Semibold/Bold) for everything UI — a modern technical grotesque with a slightly engineered character that fits a developer toolkit. **IBM Plex Mono** for code, IDs, amounts and tabular figures. Both are open-source. Headings use tight tracking (`-0.03em`); body is Regular 16/1.55.

**Spacing & shape.** 4px base rhythm. Radii are friendly-but-precise: inputs/buttons `10px`, cards `16px`, pills/avatars round. Shadows are soft and neutral — never coloured glows, no gradients in product UI.

**Motion.** Quick and functional: 120–280ms, ease `cubic-bezier(0.2,0,0.2,1)`. No bounce, no infinite loops.

**Voice.** Plain, confident, technical. EtlKit talks about what it does for data engineers — readable, testable, trustworthy pipelines — without hype.

---

## INDEX

**Foundations**
- `styles.css` — global entry point (link this). `@import`s everything below.
- `tokens/colors.css` · `typography.css` · `spacing.css` · `fonts.css` · `base.css`
- `guidelines/*.card.html` — specimen cards (Brand, Colors, Type, Spacing).

**Assets**
- `assets/logo/` — mark (vermillion / ink / white), avatar disc, favicon PNGs, lockup.

**Skill**
- `SKILL.md` — portable wrapper for this design system.

**Archive**
- `explorations/` — the icon exploration, studio iterations and finalist vote that led to the chosen mark. Reference only.
- `uploads/` — original source files, including the heritage EtlBox marks (`logo_orig*`, `logo_bw*`).
