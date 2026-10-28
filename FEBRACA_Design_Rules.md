# FEBRACA Design Rules

**The global design language for anything built for FEBRACA — decks, documents, dashboards, interfaces, social pieces, print. It governs the surfaces that carry identity: chrome, type and the mark. Colour that carries meaning rather than identity is a scoped exception, defined under Colour below. Self-contained: this file is about design, not about how code is named or structured.**

**Source:** `ManualDeMarca-Simples.pdf`, in `/Manual` — *Manual da Identidade Visual*, 23 pp., A4 landscape, Adobe Illustrator, dated 2026-01-05. Page numbers below are PDF pages, not printed folios (the manual's own cross-references are off by two).

**Authority:** the manual is the source of truth. Every rule below cites its provenance — a manual page, or a dated `**Ruling:**` where FEBRACA decided something the manual left open. A ruling outranks any reading of the manual, and marks a rule the manual doesn't contain yet; what its next edition should add is kept in `Manual-Feedback.md`. Anything still undecided is marked `**Gap:**` and must be raised, not improvised. The manual states its own standardisation is non-negotiable (p.2) — treat divergence as an error to report, not a style choice.

**Language:** prose here is English. Brand copy, colour role names in Portuguese, and the descriptor lockup are recorded verbatim and are never translated in output.

---

## Colour

CMYK for print. RGB/Hex for anything shown on a screen — social, web, video (p.8).

### 🔹Palette

Five values. Hex and CMYK are from p.8. **Ruling:** 2026-08-04 assigns the roles below — the manual states none. English names are labels for reference in code and conversation; the manual assigns none either.

- `#212B5E` → **Navy — primary.** Carries the FEBRACA name in the wordmark, and the descriptor. Also body copy throughout the manual.
- `#F79A22` → **Orange — primary.** Carries the *pata* and the vertical divider rule. The only warm value in the system.
- `#FFFFFF` → **White.** Default background. Also carries the name in place of navy **when the background is blue or black**.
- `#263882` → **Royal Blue — secondary.** **Use situation:** blue-on-blue only, where a blue image meets a blue background and the two need separating. Not a substitute for navy on type.
- `#0B0D14` → **Near-Black.** Background value. Rich black, not `#000000` — never substitute pure black. Triggers the white-name rule above.

The two primaries are the mark: navy on the name, orange on the *pata*. Only the name swaps to white, and only for contrast against blue or black — the *pata* stays orange.

CMYK equivalents for print, same page: `#212B5E` → `65 54 0 63` · `#F79A22` → `0 38 86 3` · `#FFFFFF` → `0 0 0 0` · `#263882` → `71 57 0 49` · `#0B0D14` → `45 35 0 92`.

**Gap:** no tints or shades. Do not derive tints by lightening hex values — ask. The translucent white under *Interface Guides* is the one exception. Semantic colour is not a palette gap; see below.

### 🔹Chrome vs. meaning

**Ruling:** 2026-08-04. Two kinds of colour decision exist, and only one is governed by the palette.

**Chrome — palette applies.** Colour that carries identity rather than information: headers, navigation, menus, sidebars, buttons, backgrounds, borders, and chart series used only to tell categories apart. This is what composes the global design, and it has to sit with the logo. The interface neutrals under *Interface Guides* count as part of the palette for chrome. **e.g.:** a bar chart in navy and orange; a primary button in navy.

**Meaning — free choice.** Colour that carries a convention the reader already holds: negative values, errors, success, warnings, links, diffs, statuses. The convention outranks the palette. A loss reads red and a gain reads green — do not push a gain into brand blue because blue is on-brand, since that destroys the signal the colour existed to send. *Interface Guides* gives the starting set.

**The test:** would the reader lose information if the hue changed? Yes → it is meaning, leave it conventional. No → it is chrome, use the palette.

**What this rule exists to prevent:** an interface whose logo is navy and whose menu is bright red. Semantic colour is permitted as an accent inside content; it never spreads into chrome.

### 🔹Semantic collisions

- Brand orange `#F79A22` sits in amber territory. Where warnings and chrome both appear, split them by role — orange for chrome, a visibly different amber for warnings — or drop one of the two.
- Red is a valid error and negative-value colour, but never on the logo or any of its elements. A recoloured red mark is an explicit failure case (p.12).
- Green has no relative in the palette. Keep a semantic green muted so it does not compete with the two primaries.
- **Use situation:** where something is both structural and semantic — a KPI tile that is a main surface *and* signals a negative — the surface stays brand and the signal goes on the number, not the panel.

---

## Typography

### 🔹Declared families

Two weights of one family, chosen because they harmonise while giving dynamics and contrast (p.11):

- `Knockout 49 Liteweight` → **Display:** the heavier of the two. **e.g.:** page titles, `#TransformarParaImpactar`.
- `Knockout 29 Junior Liteweight` → **Secondary display:** the narrower cut. **e.g.:** subheads, supporting lines.

Knockout is a Hoefler&Co. licensed face. Confirm a licence covers the medium before specifying it for web embedding or a third-party deliverable.

### 🔹Where Knockout is required

**Ruling:** 2026-08-04. Knockout is not mandatory for all text. It is required where FEBRACA itself is the subject — the brand speaking as the brand. **e.g.:** the logo, the website logo lockup, the organisation's bio, the name set as display type, headline claims about FEBRACA.

Everything else — running body copy, tables, captions, documentation, UI chrome — is not bound to Knockout. Choose for legibility in the medium and stay consistent within the piece.

The practical test: if replacing the text with a competitor's name would be wrong, it is brand voice and takes Knockout. If it would merely be inaccurate, it is body copy and does not.

### 🔹Body copy

No text face is declared. The manual's own body copy is set in `Neue Haas Grotesk Display Pro` (55 Roman / 75 Bold), which appears in the embedded font table but is never named as a brand asset — so it is the manual's typesetting choice, not a standard to inherit.

**Ruling:** 2026-10-28. Functional surfaces — dashboards, forms, tools — use the system font stack: nothing to download, and fast on slow mobile connections. Institutional pieces — those that tell FEBRACA's history or its work — get a face chosen with care for the piece, alongside Knockout where the brand speaks as itself. **Gap:** no house body face is declared for institutional pieces.

---

## Logo

### 🔹Construction (p.6)

The mark is built from three elements, each with a fixed meaning: the **FEBRACA** wordmark; the **outline of Brazil**, for national reach and articulation across every state; the **paw**, for the animal cause with a focus on frontline organisations. The Brazil outline is drawn as a stroked outline in the lockups and solid in the construction diagram — use the outline version. The assets in `./Assets` combine these elements in many ways, and not every asset carries all three; `FEBRACA-brand-assets-catalog.md` says what each one is.

The descriptor is always the three stacked lines `FEDERAÇÃO` / `BRASILEIRA` / `DA CAUSA ANIMAL`, all caps, navy, separated from the wordmark by a thin orange vertical rule.

### 🔹Approved versions (p.7)

The approved versions live in this repository, [FEBRACA/Brand-Assets-Catalog](https://github.com/FEBRACA/Brand-Assets-Catalog), as SVG files in `./Assets`. `FEBRACA-brand-assets-catalog.md` describes every one of them.

Always use the original file. Never reconstruct the mark from the palette, the construction description or memory, and never trace it from a screenshot or another piece of material — an invented logo is worse than a missing one.

**Precedence:** the manual governs the rules; the catalog governs which files exist. Where they disagree on what a version is called or whether it is available, the catalog wins. Where they disagree on how a version may be used, the manual wins.

### 🔹Invariants (p.12)

The logo is never altered in colour, layout, or proportion. The manual illustrates six states — one correct and five failures, each of which is a standing prohibition:

- Do not recolour any element. **e.g.:** the failure case recolours the paw and wordmark red.
- Do not change the proportion between elements. **e.g.:** shrinking the symbol relative to the type.
- Do not deform — scale uniformly, never stretch on one axis.
- Do not substitute the typeface, including for the descriptor.
- Do not change the spacing between elements.

### 🔹Positive, negative, monochrome (p.9–10)

Institutional colour is preferred. Where reproduction prevents it, the mark may run positive or negative, or in greyscale. In greyscale, pair the lighter tone with the darker background or the reverse — whichever yields the greater contrast.

### 🔹Clear space (p.14)

**Ruling:** 2026-08-18. Clear space is per asset. Each entry in `FEBRACA-brand-assets-catalog.md` carries a **Raw Margin Proportion**. That figure is raw, not the margin — **the real margin is 1/2 of it**: raw `40%` → `20%`, raw `30%` → `15%`.

Apply the real ratio to the rendered **height** of the logo's full bounding box — symbol and descriptor included — and keep that space clear on all four sides. Nothing may intrude, regardless of application.

**Ruling:** 2026-10-28. The bounding box is the file's own frame, not the drawing inside it: blank space already inside a file does not count toward the margin. When an asset needs more or less room, change its Raw Margin Proportion in the catalog.

**If the asset declares no Raw Margin Proportion**, use `20%` of the **shorter side** of the rendered bounding box — whichever of width or height is smaller — on all four sides. This fallback is already the real value, no need to change it.

Always express clear space as a ratio of the rendered mark, never a fixed value, so the margin scales with it.

### 🔹Minimum size (p.13)

`30 mm` **height** is the reduction floor for the horizontal lockup in off-set print — the dimension arrow on p.13 is vertical, on the bounding box. The manual notes the real limit also depends on the process, the quality of the original, and the quality of the reproduction, so treat `30 mm` as a floor, not a target.

Paired with the clear-space ratio above, the minimum footprint in print is `30 mm` of logo plus that asset's own clear space on each side — `6 mm` for an asset whose raw value is `40%`.

**Gap:** no minimum is given in pixels for screen, and none for any other asset in the catalog.

### 🔹Backgrounds (p.15)

White or the institutional colours only. Never place the mark on a background with insufficient contrast for legibility. **Gap:** no rule for photographic backgrounds, and no stated contrast threshold for the mark.

---

## Voice and positioning

Not decoration — these constrain copy written alongside the visual identity.

### 🔹Tone of voice (p.5)

FEBRACA balances warmth with political vision: the firm voice that organises and the extended hand that supports. Communication is **encouraging** toward ONGs and **assertive** toward partners and public officials. Register follows audience — never flatten the two into one voice.

### 🔹Archetypes (p.3)

- `CRIADOR` → **Creator:** innovation and lasting legacy.
- `CUIDADOR` → **Caregiver:** care, protection, education.
- `GOVERNADOR` → **Ruler:** order, organisation, leadership.

### 🔹Positioning (pp.2–4)

- **Purpose:** *Conectar, apoiar e representar a causa animal do Brasil* — through institutional strengthening of ONGs and the articulation of effective public policy.
- **Differentiator:** the only organisation focused on national advocacy paired with specialised mentoring.
- **Values:** Compromisso (Resultado), Transparência (Dados), Colaboração (Rede), Inovação (Futuro).
- **Audiences:** ONGs, individual animal protectors, public officials.
- **Hashtag:** `#TransformarParaImpactar`, set in Knockout as display type.

The manual positions the brand as the maximum authority on the animal cause in Brazil, operating from the National Congress to the field. Copy should not undercut that register.

---

## Contrast

**Ruling:** 2026-10-28. Text and controls follow WCAG 2.2 AA: `4.5:1` for text (`3:1` for large text) and `3:1` for interface edges. The logo is exempt, as WCAG exempts logotypes. In practice: orange never sets text, or the only edge of a control, on white.

Computed from the five declared values with the WCAG 2.2 relative-luminance formula, 2026-10-13 — derived, not a manual value.

- `#212B5E` on `#FFFFFF` → **13.36:1.** Navy on white.
- `#FFFFFF` on `#0B0D14` → **19.41:1.**
- `#FFFFFF` on `#263882` → **10.66:1.**
- `#F79A22` on `#0B0D14` → **8.87:1.**
- `#F79A22` on `#212B5E` → **6.11:1.**
- `#F79A22` on `#263882` → **4.87:1.**
- `#F79A22` on `#FFFFFF` → **2.19:1.** Below both thresholds: never text or a control's only edge on white.
- `#212B5E` with `#0B0D14` → **1.45:1**, `#263882` with `#0B0D14` → **1.82:1**, `#212B5E` with `#263882` → **1.25:1.** Surfaces that meet, never text on one another.

---

## Interface Guides

**Ruling:** 2026-10-28. Starting points for screens, not locks: every project begins here, and may leave a value when it has a reason, noting why. None of these values is brand.

### 🔹Semantic colours

Each reaches at least `5.9:1` on white, and the warning is kept visibly apart from brand orange (see *Semantic collisions*).

- `#C0271F` → **Error.** 5.91:1 on white.
- `#2F6B4F` → **Success.** 6.29:1 on white.
- `#8A5A00` → **Warning.** 5.93:1 on white.

### 🔹Outcome tones

The hue follows what the reader should do next, not how bad the news is.

- **Red** → something failed, and acting may fix it.
- **Amber** → nothing failed; wait or take note. **e.g.:** no seats left, too many attempts, a postal code not found.
- **Navy** → neutral or good news. **e.g.:** already registered.
- **Green** → done.

### 🔹Neutrals

Achromatic greys for borders, sunken surfaces and secondary text. They count as palette for chrome (see *Chrome vs. meaning*).

- `#F5F5F6`, `#EDEDEF` → **Surfaces.**
- `#D8D8DA` → **Borders.**
- `#8C8C8C` → **Interface edges only.** 3.36:1 on white: enough for an edge, never for text.
- `#5E5E66` → **Secondary text.** 6.42:1 on white.

### 🔹Translucent white

White at `8%` over navy, for boxes and backdrops that sit on a navy surface. It reads as white over navy, not as a new value, and is the one exception to the *Gap* on tints.
