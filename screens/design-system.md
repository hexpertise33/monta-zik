---
name: Electric Stage
colors:
  surface: '#131316'
  surface-dim: '#131316'
  surface-bright: '#39393c'
  surface-container-lowest: '#0e0e11'
  surface-container-low: '#1b1b1e'
  surface-container: '#1f1f22'
  surface-container-high: '#2a2a2d'
  surface-container-highest: '#353438'
  on-surface: '#e4e1e6'
  on-surface-variant: '#c4c9ac'
  inverse-surface: '#e4e1e6'
  inverse-on-surface: '#303033'
  outline: '#8e9379'
  outline-variant: '#444933'
  surface-tint: '#abd600'
  primary: '#ffffff'
  on-primary: '#283500'
  primary-container: '#c3f400'
  on-primary-container: '#556d00'
  inverse-primary: '#506600'
  secondary: '#ffb59a'
  on-secondary: '#5a1b00'
  secondary-container: '#ff5e07'
  on-secondary-container: '#531900'
  tertiary: '#ffffff'
  on-tertiary: '#313030'
  tertiary-container: '#e5e2e1'
  on-tertiary-container: '#656464'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#c3f400'
  primary-fixed-dim: '#abd600'
  on-primary-fixed: '#161e00'
  on-primary-fixed-variant: '#3c4d00'
  secondary-fixed: '#ffdbce'
  secondary-fixed-dim: '#ffb59a'
  on-secondary-fixed: '#370e00'
  on-secondary-fixed-variant: '#802a00'
  tertiary-fixed: '#e5e2e1'
  tertiary-fixed-dim: '#c8c6c5'
  on-tertiary-fixed: '#1c1b1b'
  on-tertiary-fixed-variant: '#474746'
  background: '#131316'
  on-background: '#e4e1e6'
  surface-variant: '#353438'
typography:
  headline-xl:
    fontFamily: Anton
    fontSize: 80px
    fontWeight: '400'
    lineHeight: 88px
    letterSpacing: 0.02em
  headline-lg:
    fontFamily: Anton
    fontSize: 48px
    fontWeight: '400'
    lineHeight: 52px
    letterSpacing: 0.02em
  headline-lg-mobile:
    fontFamily: Anton
    fontSize: 36px
    fontWeight: '400'
    lineHeight: 40px
    letterSpacing: 0.02em
  headline-md:
    fontFamily: Anton
    fontSize: 32px
    fontWeight: '400'
    lineHeight: 36px
  body-lg:
    fontFamily: Hanken Grotesk
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 28px
  body-md:
    fontFamily: Hanken Grotesk
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  label-md:
    fontFamily: Hanken Grotesk
    fontSize: 14px
    fontWeight: '700'
    lineHeight: 16px
    letterSpacing: 0.1em
  label-sm:
    fontFamily: Hanken Grotesk
    fontSize: 12px
    fontWeight: '600'
    lineHeight: 14px
spacing:
  unit: 8px
  gutter: 24px
  margin-mobile: 20px
  margin-desktop: 64px
  section-gap: 120px
---

## Brand & Style

The brand personality for this design system is "Amplified Energy." It is designed for a contemporary music school that bridges the gap between professional discipline and the raw emotion of a live performance. The target audience includes aspiring musicians, teenagers, and adult learners who resonate with rock, pop, and electronic music culture.

The design style is **High-Contrast / Bold** with a secondary influence of **Minimalism**. It mimics the atmosphere of a concert stage: deep, dark voids punctuated by intense, focused light. The UI should evoke an immediate sense of movement, rhythm, and passion. Expect large-scale typography, aggressive color transitions, and a clean but "edgy" aesthetic that prioritizes high-impact visuals and photography of instruments in action.

## Colors

The palette is strictly dark-mode to simulate the "backstage" and "on-stage" experience. 

- **Primary (Electric Lime):** A high-visibility, high-frequency yellow-green used for primary actions and key highlights. It represents the "energy" of the school.
- **Secondary (Ignite Orange):** Used for secondary accents, notifications, or to denote "heat" and passion. It provides a warm counterpoint to the primary lime.
- **Background (Charcoal Deep):** A layered set of near-blacks. The base background is `#0F0F12`, while surface elements use `#1A1A1A`.
- **Contrast:** Text should primarily be white (`#FFFFFF`) or high-level grey for maximum legibility against the dark surfaces. Primary actions use the Primary color with black text for "vibrating" contrast.

## Typography

The typography system uses a "Power and Precision" pairing. 

**Headlines** use **Anton** for an impactful, condensed, and urgent feel. It should be treated as a graphical element—don't be afraid to use it at very large scales (headline-xl) for hero sections. Headlines are always uppercase to maintain the "rock" aesthetic.

**Body text and Labels** use **Hanken Grotesk**. This provides a sharp, contemporary, and highly legible contrast to the heavy headers. It ensures that professional information (schedules, pricing, curriculum) remains easy to digest. Labels are set in bold, uppercase with increased letter spacing to act as "functional markers" in the UI.

## Layout & Spacing

This design system utilizes a **Fluid Grid** with generous vertical breathing room to allow high-impact photography to shine.

- **Grid:** A 12-column grid for desktop, 8-column for tablet, and 4-column for mobile.
- **Rhythm:** An 8px base unit drives all spacing. 
- **Verticality:** Use large `section-gap` tokens (120px+) to separate distinct content areas. This creates a "breath" between the intensity of different sections.
- **Visual Tension:** Align text strictly to the grid but allow "hero" images of instruments to occasionally break the container or bleed off the edge of the screen to create a dynamic, unconfined feel.

## Elevation & Depth

To maintain the "Stage" feel, depth is created through **Tonal Layers** rather than soft shadows. 

- **Surface Levels:** The background is the deepest layer. Cards and containers sit one step above (`#1A1A1A`). 
- **Light Accents:** Instead of shadows, use "Rim Lighting"—1px inner borders or top-strokes in a low-opacity white (10-15%) to define the edges of dark elements against dark backgrounds.
- **Glow Effects:** Reserve "Glow" (outer blurs) specifically for the Primary color to simulate neon or stage lights. Use a concentrated, high-intensity glow for active states and "Live" indicators.
- **Photography:** Images should use a slight dark gradient overlay at the bottom or top to ensure white typography remains legible.

## Shapes

The shape language is **Sharp (0)**. 

To emphasize the "edgy" and "rock" vibe, the design system avoids rounded corners. Square edges on buttons, inputs, and cards convey a sense of precision and professional architectural strength. 

**Exceptions:** 
- Interactive "Play" buttons or specific icons may use circular containers to denote their unique function.
- Decorative angled clips (e.g., a 45-degree cut on one corner of a card) can be used to add a "custom-build" or "industrial" feel to the UI.

## Components

- **Buttons:** Primary buttons are rectangular with the Primary color background and black text. Hover states should invert or shift to the Secondary color. Use large, bold uppercase text.
- **Input Fields:** Dark background (`#1A1A1A`) with a bottom-only border in white. When focused, the bottom border transitions to the Primary Electric color.
- **Cards:** No borders, solid dark grey background. Use "Rim Lighting" (1px subtle top border) to separate them from the main background. All images within cards should have a "duotone" or high-contrast black and white filter that reveals full color on hover.
- **Chips/Badges:** Small, rectangular, and high-contrast. Used for tagging music genres (e.g., "ROCK", "METAL", "JAZZ").
- **Progress Bars (Metronome/Learning):** High-intensity lime green bars against a pitch-black track.
- **Lists:** Clean lines with thin dividers (`rgba(255,255,255,0.1)`). Use the primary color for bullets or numbers.
- **The "Stage" Component:** A specialized full-width hero component designed to hold a background video or high-energy photo of a performer, with a Headline-XL overlay.