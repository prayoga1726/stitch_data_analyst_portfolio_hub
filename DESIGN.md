---
name: Organic Logic
colors:
  surface: '#f0fde9'
  surface-dim: '#d1decb'
  surface-bright: '#f0fde9'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#ebf7e4'
  surface-container: '#e5f2de'
  surface-container-high: '#dfecd8'
  surface-container-highest: '#dae6d3'
  on-surface: '#141e12'
  on-surface-variant: '#4b463e'
  inverse-surface: '#283326'
  inverse-on-surface: '#e8f5e1'
  outline: '#7d766d'
  outline-variant: '#cec5bb'
  surface-tint: '#665d4e'
  primary: '#665d4e'
  on-primary: '#ffffff'
  primary-container: '#ecdfcc'
  on-primary-container: '#6b6253'
  inverse-primary: '#d1c5b3'
  secondary: '#5e5f58'
  on-secondary: '#ffffff'
  secondary-container: '#e4e3da'
  on-secondary-container: '#64655e'
  tertiary: '#5c6055'
  on-tertiary: '#ffffff'
  tertiary-container: '#dfe2d5'
  on-tertiary-container: '#61655a'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#eee1ce'
  primary-fixed-dim: '#d1c5b3'
  on-primary-fixed: '#211b0f'
  on-primary-fixed-variant: '#4e4638'
  secondary-fixed: '#e4e3da'
  secondary-fixed-dim: '#c7c7bf'
  on-secondary-fixed: '#1b1c17'
  on-secondary-fixed-variant: '#464741'
  tertiary-fixed: '#e1e4d7'
  tertiary-fixed-dim: '#c4c8bb'
  on-tertiary-fixed: '#191d15'
  on-tertiary-fixed-variant: '#44483f'
  background: '#f0fde9'
  on-background: '#141e12'
  surface-variant: '#dae6d3'
typography:
  headline-xl:
    fontFamily: Hanken Grotesk
    fontSize: 48px
    fontWeight: '700'
    lineHeight: 56px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Hanken Grotesk
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
    letterSpacing: -0.01em
  headline-lg-mobile:
    fontFamily: Hanken Grotesk
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  body-md:
    fontFamily: Work Sans
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  body-sm:
    fontFamily: Work Sans
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  label-caps:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '500'
    lineHeight: 16px
    letterSpacing: 0.08em
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  unit: 4px
  gutter: 24px
  margin-mobile: 16px
  margin-desktop: 64px
  container-max: 1440px
---

## Brand & Style

The design system embodies a philosophy of **Organic Logic**. It fuses the warmth of natural materials with the rigid precision of high-end analytical tools. The goal is to create an environment that feels intellectually stimulating yet approachable—moving away from sterile, cold tech aesthetics toward a "Digital Atelier" feel.

The target audience consists of researchers, analysts, and designers who value high-density information environments but seek a more humanistic interface.

### Visual Style: Warm Professionalism
This system utilizes a **refined-minimalist** approach with a **tactile-paper** influence. 
- **Warmth:** High-key parchment backgrounds reduce eye strain and provide a sophisticated backdrop.
- **Precision:** Monospaced accents and razor-sharp borders signify technical rigor.
- **Clarity:** Generous white space (or "parchment space") is used to prevent cognitive overload in data-heavy views.

## Colors

The palette is built around the tension between the organic warmth of `#ECDFCC` and the deep, structural slate of `#181C14`.

- **Primary (#ECDFCC):** Used for large surfaces, card backgrounds, and main UI containers in light mode. It acts as the "paper" of the interface.
- **Secondary (#3C3D37):** A deep charcoal with a slight olive undertone. Used for secondary text, iconography, and subtle borders.
- **Tertiary (#181C14):** The "ink." Used for high-contrast headlines, primary buttons, and deep background layers in dark mode.
- **Neutral (#697565):** A sage-tinted slate used for disabled states, meta-data, and instructional text.

**Dark Mode Implementation:**
In dark mode, the hierarchy inverts. `#181C14` becomes the base surface. `#ECDFCC` shifts from a background color to a high-contrast accent for primary actions and critical highlights, maintaining its warmth against the dark void.

## Typography

The typography system balances contemporary geometry with technical utility. 

- **Headlines:** Uses **Hanken Grotesk** for a sharp, modern feel. Tracking is tightened slightly in larger sizes to maintain a compact, authoritative appearance.
- **Body:** **Work Sans** provides a grounded, neutral reading experience. Its high x-height ensures legibility against the textured parchment backgrounds.
- **Labels & Data:** **JetBrains Mono** is reserved for metadata, small labels, and numerical data. This reinforces the "Precision" aspect of the design narrative, making utilitarian information look intentional and calculated.

## Layout & Spacing

This design system utilizes a **strictly structured 8px grid** to ensure the "Logic" portion of the narrative is physically felt.

- **Layout Model:** A 12-column fluid grid for desktop with fixed margins of 64px. For tablet, this reduces to 8 columns with 32px margins. Mobile uses a 4-column layout with 16px margins.
- **Rhythm:** Vertical rhythm is maintained by keeping all component heights and vertical margins as multiples of 8px. 
- **Content Density:** High-density data tables should use 4px (half-unit) internal padding, while editorial or landing pages should use 32px or 48px blocks to emphasize the parchment surface.

## Elevation & Depth

To maintain the "Organic" feel, this design system avoids heavy, artificial drop shadows. Instead, it uses **Tonal Layers** and **Micro-borders**.

- **Surface Tiering:** Depth is communicated by shifting the background color slightly. Level 0 is the base parchment; Level 1 (cards) uses a 2% darker or lighter tint; Level 2 (modals) uses a crisp 1px solid border in the secondary color.
- **Shadows:** When shadows are necessary for focus (e.g., dropdowns), use "Ambient Tints." Instead of pure black shadows, use a highly diffused `#181C14` shadow at 5-8% opacity to maintain a natural, soft appearance.
- **Ghost Borders:** Use 1px borders in the neutral shade (`#697565`) at 20% opacity for structural separation without adding visual weight.

## Shapes

The shape language is **Soft (0.25rem)**. This slight rounding takes the "edge" off the brutalist structure, making the interface feel crafted rather than manufactured.

- **Interactive Elements:** Buttons and input fields use the standard `rounded` (4px).
- **Large Containers:** Cards and modals use `rounded-lg` (8px) to provide a gentle container for the data within.
- **Selection States:** Tabs and active menu items use a sharp 2px rounding to emphasize precision.

## Components

### Buttons
- **Primary:** Solid `#181C14` with `#ECDFCC` text. Sharp corners (4px). On hover, the background shifts to `#3C3D37`.
- **Secondary:** Outlined 1px in `#3C3D37` with no fill.
- **Tertiary:** Text-only using the Monospaced label font to signal a technical action.

### Input Fields
- Use a "Base-line" style or a very subtle filled style. The background should be a 5% darker tint of the parchment. 
- Focus state: A 2px solid border on the left side using the primary color to indicate activity without surrounding the entire element.

### Cards
- Cards should not have shadows. Instead, use a 1px solid border in `#3C3D37` at 10% opacity. 
- For "Active" cards, increase the border opacity to 100% and use the monospaced label in the top right corner as an identifier.

### Chips & Tags
- Rounded-pill shapes using `#697565` at low opacity with the monospaced font. These should look like small stamps or mechanical labels.

### Data Tables
- Horizontal lines only. Use `#3C3D37` at 15% opacity. 
- Header rows should use the `#ECDFCC` color as a background to invert the logic and draw the eye to the data structure.