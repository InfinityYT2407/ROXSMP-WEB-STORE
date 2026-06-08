---
name: Premium Minecraft Store Design System
colors:
  surface: '#131313'
  surface-dim: '#131313'
  surface-bright: '#393939'
  surface-container-lowest: '#0e0e0e'
  surface-container-low: '#1c1b1b'
  surface-container: '#201f1f'
  surface-container-high: '#2a2a2a'
  surface-container-highest: '#353534'
  on-surface: '#e5e2e1'
  on-surface-variant: '#bbcbb4'
  inverse-surface: '#e5e2e1'
  inverse-on-surface: '#313030'
  outline: '#869580'
  outline-variant: '#3d4a39'
  surface-tint: '#3ae449'
  primary: '#54f95b'
  on-primary: '#003907'
  primary-container: '#2ddb41'
  on-primary-container: '#005a10'
  inverse-primary: '#006e16'
  secondary: '#fff9ef'
  on-secondary: '#3a3000'
  secondary-container: '#ffdb3c'
  on-secondary-container: '#725f00'
  tertiary: '#dcdad9'
  on-tertiary: '#313030'
  tertiary-container: '#c0bebd'
  on-tertiary-container: '#4e4d4d'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#72ff70'
  primary-fixed-dim: '#3ae449'
  on-primary-fixed: '#002203'
  on-primary-fixed-variant: '#00530e'
  secondary-fixed: '#ffe16d'
  secondary-fixed-dim: '#e9c400'
  on-secondary-fixed: '#221b00'
  on-secondary-fixed-variant: '#544600'
  tertiary-fixed: '#e5e2e1'
  tertiary-fixed-dim: '#c8c6c5'
  on-tertiary-fixed: '#1c1b1b'
  on-tertiary-fixed-variant: '#474746'
  background: '#131313'
  on-background: '#e5e2e1'
  surface-variant: '#353534'
typography:
  display-lg:
    fontFamily: Sora
    fontSize: 48px
    fontWeight: '800'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  display-lg-mobile:
    fontFamily: Sora
    fontSize: 32px
    fontWeight: '800'
    lineHeight: '1.2'
  headline-md:
    fontFamily: Sora
    fontSize: 24px
    fontWeight: '700'
    lineHeight: '1.3'
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  label-sm:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '500'
    lineHeight: '1'
    letterSpacing: 0.05em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  base: 8px
  xs: 0.25rem
  sm: 0.5rem
  md: 1rem
  lg: 2rem
  xl: 4rem
  container-max: 1280px
  gutter: 24px
---

## Brand & Style

The design system is engineered for a high-end, immersive Minecraft marketplace experience. It moves away from traditional voxel-based aesthetics toward a sophisticated "Dark Gaming" style. The brand personality is professional, authoritative, and rewarding, aiming to evoke the excitement of high-tier loot and prestigious ranks.

The visual direction utilizes **Glassmorphism** combined with a **Corporate Modern** layout structure. By using translucent surfaces, subtle background blurs, and luminous accents, the UI feels deep and layered. This approach maintains a "tech" feel appropriate for a server network while ensuring the "Minecraft" influence is felt through color and light rather than literal block shapes.

## Colors

The palette is anchored in a deep charcoal foundation to allow luminous accents to pop. 

*   **Primary (Emerald Green):** Reserved for high-priority actions, successful purchase indicators, and primary CTAs. It should feel vibrant and "charged."
*   **Secondary (Gold):** Used exclusively for premium ranks, limited-time offers, and "Legendary" tier items to signify value and prestige.
*   **Neutral (Charcoal/Black):** The base layer is a true dark #121212, while surfaces utilize a lighter #1A1A1A with varying opacity to create depth.
*   **Status Colors:** Use standard reds for errors, but ensure they are saturated enough to stand out against the dark background.

## Typography

This design system uses a hierarchical font strategy to balance gaming energy with readability.

*   **Headlines (Sora):** A geometric sans-serif with a technical edge. Use "Extra Bold" for page titles to command attention.
*   **Body (Inter):** The workhorse font. High legibility for item descriptions and terms of service.
*   **Labels (JetBrains Mono):** Used for technical data, quantities, server IP displays, and small badges. The monospaced nature reinforces the "digital/code" aspect of Minecraft.

All typography should favor high contrast (White or light grey) against the dark background. Use `uppercase` with increased letter spacing for `label-sm` to create a premium, "metered" look.

## Layout & Spacing

The design system utilizes a **fluid 12-column grid** for desktop, collapsing to a single column for mobile. 

*   **Rhythm:** An 8px base unit drives all padding and margins. 
*   **Margins:** Use large `xl` (64px) vertical spacing between major sections (e.g., Category Rows) to maintain a premium, "uncluttered" feel.
*   **Safe Areas:** Desktop layouts should have a 24px gutter to ensure glass elements have enough breathing room to show background blurs.
*   **Mobile:** Reduce `display-lg` sizes significantly and switch to a 16px gutter to maximize screen real estate for item cards.

## Elevation & Depth

Depth is not communicated through traditional drop shadows, but through **Tonal Layering** and **Backdrop Blurs**.

1.  **Level 0 (Background):** Solid #121212.
2.  **Level 1 (Card/Container):** Semi-transparent #1A1A1A (opacity 0.6) with a `backdrop-filter: blur(12px)`.
3.  **Level 2 (Hover State):** Increase opacity and add an "Inner Glow" (a 1px semi-transparent border) using the primary Emerald or Gold color.
4.  **Glows:** Use `box-shadow` with high blur (40px+) and low opacity (0.2) using the accent color to simulate a light source emitting from premium items or active progress bars.

## Shapes

To maintain the "Professional" directive, the design system avoids 0px sharp corners (too aggressive) and pill-shapes (too casual). 

The `rounded-md` (0.5rem) is the standard for cards and input fields. `rounded-lg` (1rem) should be reserved for large modal containers or hero image sections. This provides a soft, modern touch that contrasts beautifully with the technical typography.

## Components

### Buttons
*   **Primary:** Solid Emerald Green (#2DDB41) with black text for maximum contrast. On hover, add a subtle outer glow of the same color.
*   **Secondary:** Ghost style (transparent background) with a 1px white border.
*   **Premium:** Gradient background from Gold (#FFD700) to a deeper amber.

### Item Cards
*   Glassmorphic background.
*   1px border (top and left) slightly lighter than the background to simulate a light source.
*   Hover state: Card scales 2% and the border color changes to Emerald Green.

### Progress Bars (Donation Goals)
*   Track: Dark charcoal with an inner shadow.
*   Fill: Emerald Green gradient.
*   Effect: Add a "pulse" animation to the fill if the goal is >90% complete.

### Badges & Ranks
*   Utilize `JetBrains Mono` for text.
*   Backgrounds should be high-saturation colors with a low-opacity "glow" behind them to denote rarity (e.g., Purple for Epic, Gold for Legendary).

### Input Fields
*   Dark, semi-transparent backgrounds. 
*   Active state: The bottom border glows Emerald.