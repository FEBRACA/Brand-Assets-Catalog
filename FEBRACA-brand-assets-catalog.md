# FEBRACA — Brand Assets Catalog (SVG)

16 vector files, verified by inspection and rendering. All type is outlined, no live strokes, no embedded rasters.

**Naming rule applied:** `febraca-<role>-<variant>[-<modifier>]`
`role` = `logo` · `card` · `badge` · `icon` · `campaign` · `pattern`.
All lowercase, hyphen-separated, no accents, no spaces, no underscores — safe in raw URLs. Files are saved in `./Assets/[format svg, png...]`

---

## Horizontal lockups

### `febraca-logo-horizontal-notag` / `logo_sem_tag`

Icon at left, "FEBRACA" wordmark at right, no descriptor. The compact primary lockup.
For site headers, presentation footers, narrow strips and anywhere the full name is already established.
Ratio 2.97:1 · landscape · transparent background. Raw Margin Proportion: 40%

### `febraca-logo-horizontal-tagline` / `logo_vertical`

Icon at left; wordmark on top with the three-line descriptor stacked beneath it, after the orange rule.
The standard institutional lockup — documents, letterheads, reports, official materials.
Ratio 2.70:1 · landscape despite the old "vertical" filename · transparent background. Raw Margin Proportion: 40%

### `febraca-logo-horizontal-wide-tagline` / `logo_centralizado`

Single-line band: wordmark at left, icon in the middle, orange rule, then the descriptor at right.
The widest asset in the set — email signatures, banner strips, website footers, event backdrops.
Ratio 4.20:1 · landscape · transparent background. Raw Margin Proportion: 40%

## Square lockups

### `febraca-logo-square-notag` / `logo_quadrado`

Icon at left with the wordmark broken across three lines (FE / BRA / CA), no descriptor.
For square and portrait spaces where the horizontal lockup would render too small — social posts, tote bags, signage.
Ratio 1.29:1 · landscape · transparent background.

### `febraca-logo-square-tagline` / `logo_verticalizado`

Same construction as above, with the three-line descriptor added below after the orange rule.
The square counterpart of the institutional lockup, for feed posts and covers that need the full name.
Ratio 1.07:1 · near-square, slightly landscape — not portrait as the old filename suggests · transparent background.

## Cards and badge

### `febraca-card-square-flat` / `selo_card_flat`

Stacked lockup — solid navy map with orange pata above, wordmark and descriptor below — on a plain field.
Flat and unframed: profile pictures, avatars, app tiles, sticker sheets.
Ratio 1:1 · background is part of the artwork (`#FFFFFF`), not transparent.

### `febraca-card-square-framed` / `selo_card`

Same stacked lockup on a rounded card, enclosed by a navy border with an orange accent frame offset behind it.
The dressed version — certificates, printed cards, presentation opening slides, member kits.
Ratio 1:1 · background is part of the artwork (`#FFFFFF`), not transparent.

### `febraca-badge-circular` / `logo_redondo`

Circular seal: outlined map with orange pata at the center, full institutional name set around the ring.
Formal seal applications — certificates, stamps, medals, member seals, stickers.
Ratio 0.91:1 · transparent background.

## Icons (symbol only)

### `febraca-icon-outline` / `icone`

Brazil as a navy contour with the solid orange pata sitting inside the southeast region.
Lightest visual weight in the set — watermarks, large-format backgrounds, light layouts, line-art contexts.
Ratio 0.94:1 · replaces the old `icone_-_macro_interno.png`, where the pata overhung the border.

### `febraca-icon-solid` / `icone_minimalista`

Filled navy Brazil with the orange pata placed directly on the navy, no separating contour.
Default icon at medium and large sizes, where the pata still reads clearly against the navy.
Ratio 0.98:1 · transparent background.

### `febraca-icon-solid-haloed` / `icone_minimalista_2`

The same solid symbol with a white contour separating the pata from the navy silhouette.
Safest choice at small sizes and on dark surfaces — favicons, app icons, bullets, WhatsApp.
Ratio 0.98:1 · transparent background.

## Campaign lockups

### `febraca-campaign-eu-animais` / `eu_animais`

Campaign phrase "EU [pata] ANIMAIS", the orange pata standing in for the verb, endorsed by a small icon + FEBRACA signature at lower right.
For public-facing mobilization — social campaigns, t-shirts, placards, stickers, awareness pieces.
Ratio 3.15:1 · a campaign mark, not a substitute for the institutional logo.

### `febraca-campaign-eu-ongs` / `eu_ongs`

Same construction with "ONGS" in place of "ANIMAIS" — aimed at member organizations rather than the general public.
For filiation drives, ONG-facing materials, event badges and capacity-building programs.
Ratio 2.52:1 · transparent background.

## Patterns

### `febraca-pattern-paws-orange` / `pattern_1`

Dense grid of orange patas in alternating orientation, no other motif.
The lightest and most playful of the three — accent bands, dividers, packaging, social backgrounds.
Ratio 2.91:1 · single color `#F79A22` · finished panel, not a seamless repeat tile.

### `febraca-pattern-map-outline-navy` / `pattern_2`

Tilted outlined Brazil silhouettes, each holding a solid navy pata, spaced airily.
Low-contrast and line-based — good behind text, on document covers and light presentation slides.
Ratio 2.61:1 · single color `#212B5E` · finished panel, not a seamless repeat tile.

### `febraca-pattern-map-solid-navy` / `pattern_3`

Tilted solid navy Brazil silhouettes with the pata knocked out in white, packed tightly.
The heaviest treatment — full-bleed covers, endpapers, banners, merchandise; too dense to sit behind body copy.
Ratio 2.39:1 · single color `#212B5E` · finished panel, not a seamless repeat tile.

### `febraca-logo-horizontal-wide-tagline-iconleft` / `logo`

Single-line band: icon at left, wordmark in the middle, orange rule, then the descriptor at right.
The wide lockup in reading order, led by the symbol — email signatures, banner strips, website headers and footers, event backdrops.
Ratio 4.25:1 · landscape · transparent background. Raw Margin Proportion: 40%

---

## Color palette

| Color      | Hex       | Role               | Application                                                       |
| ---------- | --------- | ------------------ | ----------------------------------------------------------------- |
| Navy       | `#212B5E` | Primary            | Wordmark, descriptor, map contour and silhouette                  |
| Orange     | `#F79A22` | Primary            | Pata, vertical divider rule — the only warm value in the system   |
| White      | `#FFFFFF` | Default background | Card fields, knocked-out pata in `febraca-pattern-map-solid-navy` |
| Royal Blue | `#263882` | Secondary          | Blue-on-blue separation only. Never a substitute for navy on type |
| Near-Black | `#0B0D14` | Background         | Rich black — never substitute `#000000`                           |
