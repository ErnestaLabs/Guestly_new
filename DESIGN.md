# Brand System: Luxury Executive Operations (Vogue / Gucci Glamour)
# Target Blueprint: Editorial Warmth + Cinema Black Authority

## 1. Design Tokens & Variables

### Color Palette
:root {
  /* Canvas & Backgrounds */
  --color-canvas-primary: #FBF9F6;    /* Vogue Cream - warm, heavy-paper stock luxury */
  --color-canvas-dark: #0D0D0D;       /* Cinema Black - true rich deep black for high contrast */
  --color-surface-card: #FFFFFF;      /* Pure crisp white for structured floating elements */
  
  /* Typography & Lines */
  --color-text-primary: #0D0D0D;      /* Deep black for high-readability on cream */
  --color-text-muted: #5A544E;        /* Gucci Espresso - soft dark brown-gray for secondary text */
  --color-text-light: #FBF9F6;        /* Cream text used when resting on dark surfaces */
  --color-border: rgba(13, 13, 13, 0.08); /* Ultra-thin, barely-there editorial lines */
  
  /* Accents (Used <2% of total layout) */
  --color-accent: #D4AF37;            /* Liquid Gold - exclusive hover states and micro-details */
}

### Typography (Editorial Monolith)
*   **Display & Headings (H1, H2, H3):** `Cormorant Garamond` or `Didot` (Serif). 
    *   *Styling:* High contrast, sharp serif, heavy usage of italicized emphasis terms. 
    *   *Spacing:* Letter spacing set to `-0.02em` for large headers; `0.1em` uppercase for subheadings.
*   **Body Text:** `Inter` or `Montserrat` (Neo-Grotesque Sans-Serif).
    *   *Styling:* Rendered small and sharp (14px–16px), tracking regular, line height generous (`line-height: 1.75`) to force whitespace breathing room.
*   **Interactive / CTAs / Navigation:** All caps, wide tracking (`letter-spacing: 0.18em`), small font weight (`font-weight: 500`).

### Spacing & Layout
*   **Section Padding:** Extreme vertical clearance. Minimum `clamp(6rem, 10vw, 12rem)` vertical padding to signal elite scarcity.
*   **Layout Grid:** Strict asymmetric split screens (50/50 blocks) and clean, offset editorial masonry. 

---

## 2. Component Specifications

### 2.1 The "Vogue Cover" Hero Section
*   **Structure:** Desktop 50/50 viewport split canvas.
    *   **Left Pane (Vogue Cream background):** Massive, screen-dominant serif header. No sub-headlines, just an authoritative statement. A single minimalist, text-only text link CTA with an ultra-thin underline.
    *   **Right Pane:** Full-bleed, high-fashion vertical portrait of the founder. 
*   **Navigation:** Absolutely positioned at top, floating, zero-background fill. Thin border bottom (`1px solid var(--color-border)`). Text-only monogram logo.

### 2.2 Asymmetric Copy Blocks (The Authority Statement)
*   **Structure:** 1-column layout restricted to `720px` max-width, offset to the left or right of the screen canvas. Large amounts of empty cream space flanking it.
*   **Style:** 32px `Cormorant Garamond` text block detailing the philosophy of scale, leverage, and executive operational partnership.

### 2.3 The Executive Tier Accordion (Instead of Service Grids)
*   **Structure:** A full-width vertical stack of expandable rows. No multi-column cards (which look like cheap SaaS templates).
*   **Interaction:** Clicking a tier opens a clean smooth container slider revealing deep scope profiles.
*   **Style:** Left side features the package Roman numeral (`SUITE I`, `SUITE II`), middle features high-ticket operational title, right side features a minimalist slide indicator icon `+`.

### 2.4 The Gatekeeper Intake Dossier (Application Form)
*   **Structure:** Dark Mode inversion section. The canvas switches entirely to `var(--color-canvas-dark)` and `var(--color-text-light)` to signal entering a private room.
*   **Inputs:** Minimalist form design. No box borders. Only a single bottom underline input line (`1px solid rgba(255,255,255,0.2)`).
*   **CTA Button:** Rigid, hard-edged solid cream block with sharp black typography. No rounded corners (`border-radius: 0px`).

---

## 3. Global UI Rules & Execution Guidelines

*   **Radical Subtraction:** Absolutely no icons from common libraries (FontAwesome, Lucide) unless they are customized, single-weight, ultra-thin vector lines. No colored backgrounds for icons.
*   **Strict Image Treatment:** All lifestyle images must utilize a subtle desaturation matrix or high-fashion warm color grading to match the Gucci Espresso palette tones.
*   **Micro-Animations:** Low-velocity transitions. Page transitions use smooth opacity scaling (`transition: all 0.5s cubic-bezier(0.25, 1, 0.5, 1)`). No bouncing, popping, or rapid tech-startup style hover motions.
