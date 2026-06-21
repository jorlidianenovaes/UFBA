---
name: Academic Excellence Framework
colors:
  surface: '#f9f9f9'
  surface-dim: '#dadada'
  surface-bright: '#f9f9f9'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f3f3f4'
  surface-container: '#eeeeee'
  surface-container-high: '#e8e8e8'
  surface-container-highest: '#e2e2e2'
  on-surface: '#1a1c1c'
  on-surface-variant: '#44474f'
  inverse-surface: '#2f3131'
  inverse-on-surface: '#f0f1f1'
  outline: '#747780'
  outline-variant: '#c4c6d0'
  surface-tint: '#435e90'
  primary: '#00183b'
  on-primary: '#ffffff'
  primary-container: '#0b2d5c'
  on-primary-container: '#7b96cb'
  inverse-primary: '#acc7ff'
  secondary: '#35618d'
  on-secondary: '#ffffff'
  secondary-container: '#a2cdff'
  on-secondary-container: '#2a5782'
  tertiary: '#161a1c'
  on-tertiary: '#ffffff'
  tertiary-container: '#2b2e31'
  on-tertiary-container: '#939598'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#d7e2ff'
  primary-fixed-dim: '#acc7ff'
  on-primary-fixed: '#001b40'
  on-primary-fixed-variant: '#2a4676'
  secondary-fixed: '#d1e4ff'
  secondary-fixed-dim: '#a0cafc'
  on-secondary-fixed: '#001d35'
  on-secondary-fixed-variant: '#184974'
  tertiary-fixed: '#e0e3e6'
  tertiary-fixed-dim: '#c4c7ca'
  on-tertiary-fixed: '#191c1e'
  on-tertiary-fixed-variant: '#44474a'
  background: '#f9f9f9'
  on-background: '#1a1c1c'
  surface-variant: '#e2e2e2'
typography:
  display-lg:
    fontFamily: Inter
    fontSize: 48px
    fontWeight: '700'
    lineHeight: 56px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
    letterSpacing: -0.01em
  headline-lg-mobile:
    fontFamily: Inter
    fontSize: 28px
    fontWeight: '600'
    lineHeight: 36px
  headline-md:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  body-lg:
    fontFamily: Source Serif 4
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 28px
  body-md:
    fontFamily: Source Serif 4
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  label-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '500'
    lineHeight: 20px
    letterSpacing: 0.05em
  caption:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '400'
    lineHeight: 16px
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  unit: 8px
  container-max: 1280px
  gutter: 24px
  margin-mobile: 16px
  margin-desktop: 48px
  section-gap: 80px
---

## Brand & Style

The design system is engineered for a high-level academic environment, specifically tailored for a Master's Thesis presentation. The brand personality is authoritative, intellectual, and visionary, reflecting the rigors of postgraduate research while embracing modern digital aesthetics.

The visual style is a hybrid of **Institutional Minimalism** and **Refined Glassmorphism**. It prioritizes clarity and information density, utilizing vast whitespace to allow complex data to breathe. The "university-grade" feel is achieved through structural precision, while subtle organic elements—like abstract waves and dotted network lines—soften the academic formality. The UI should evoke a sense of prestige, reliability, and innovative collaboration.

## Colors

The palette is rooted in deep, institutional blues to establish immediate credibility and trust. 

- **Navy Blue (#0B2D5C):** Used for primary headings, navigation bars, and heavy structural elements.
- **Institutional Blue (#1F4E79):** Used for interactive states, secondary buttons, and iconography.
- **Light Gray (#F5F7FA):** The primary background color to reduce eye strain and provide a canvas for glassmorphic layers.
- **White (#FFFFFF):** Reserved for card surfaces, content containers, and high-contrast text against dark backgrounds.

Visual accents include a "watermark" map of Seabra, rendered in a 3% opacity version of Navy Blue, appearing as a subtle background texture to ground the project in its geographical context.

## Typography

This design system utilizes a paired typographic scale to balance modern utility with classical academic readability. 

**Inter** is the primary typeface for all UI controls, headings, and data labels. Its geometric precision conveys modernity and technological integration. **Source Serif 4** is employed for long-form body text, providing the "scholarly" feel required for a thesis while ensuring high legibility for complex Portuguese syntax.

All headings use tight letter spacing for a premium "editorial" look. Labels and captions use increased tracking to maintain clarity at small sizes.

## Layout & Spacing

The layout follows a **Fixed Grid** philosophy on desktop to maintain the organized structure of a formal document. A 12-column grid is used with generous gutters to create a sophisticated, airy feel.

- **Desktop:** 1280px max-width container, centered.
- **Tablet:** 8-column fluid grid with 32px margins.
- **Mobile:** 4-column fluid grid with 16px margins; typography scales down for readability.

Vertical rhythm is governed by an 8px base unit. Sections are separated by significant "Section Gaps" (80px+) to clearly delineate different chapters or modules of the research.

## Elevation & Depth

Hierarchy is established through **Glassmorphism** and **Tonal Layering** rather than heavy shadows.

1.  **Base Layer:** Light Gray (#F5F7FA) solid background.
2.  **Mid Layer (Cards):** White (#FFFFFF) with a 40% blur (backdrop-filter: blur(20px)) and a subtle 1px border (#E1E8F0).
3.  **Top Layer (Modals/Popovers):** Pure White with a soft, expansive ambient shadow (0px 20px 40px rgba(11, 45, 92, 0.08)).

Dotted line connections ("networking lines") exist on a z-index between the base and mid-layer, visually connecting related data points without cluttering the foreground.

## Shapes

The shape language is **Organic and Purposeful**. While structural containers use a standard 0.5rem (8px) radius to maintain professional discipline, "Interactive Objects" (like buttons and active chips) and decorative "Abstract Waves" utilize much higher rounding to feel approachable.

Visual elements representing collaboration or networking should avoid sharp 90-degree angles, opting instead for smooth paths and circular nodes.

## Components

- **Academic Cards:** White backgrounds with semi-transparent glass footers. Hovering triggers a subtle lift (y-axis -4px) and an increase in the soft shadow's spread.
- **Institutional Buttons:** Primary buttons are Navy Blue with White text. Secondary buttons are Ghost-style with a 1px Institutional Blue border. Transitions must be smooth (300ms ease-in-out).
- **Dynamic Tabs:** Underline-style indicators that "slide" between states, mimicking the fluid movement of the background waves.
- **Educational Icons:** Mono-line vector icons (books, graduation caps, nodes). Use Institutional Blue for the primary stroke and a 10% opacity Navy Blue for a "soft fill" effect.
- **Navigation:** A sticky top-bar using 80% opacity White with a backdrop blur, ensuring content remains legible as it scrolls underneath.
- **Interactive Graphs:** Use dotted lines for connections and soft-rounded "dots" for data points to maintain the networking theme.