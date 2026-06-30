---
name: Alpine Velocity
colors:
  surface: '#0b1326'
  surface-dim: '#0b1326'
  surface-bright: '#31394d'
  surface-container-lowest: '#060e20'
  surface-container-low: '#131b2e'
  surface-container: '#171f33'
  surface-container-high: '#222a3d'
  surface-container-highest: '#2d3449'
  on-surface: '#dae2fd'
  on-surface-variant: '#c1c6d7'
  inverse-surface: '#dae2fd'
  inverse-on-surface: '#283044'
  outline: '#8b90a0'
  outline-variant: '#414755'
  surface-tint: '#adc6ff'
  primary: '#adc6ff'
  on-primary: '#002e69'
  primary-container: '#4b8eff'
  on-primary-container: '#00285c'
  inverse-primary: '#005bc1'
  secondary: '#c6c6c7'
  on-secondary: '#2f3131'
  secondary-container: '#454747'
  on-secondary-container: '#b4b5b5'
  tertiary: '#ffb59a'
  on-tertiary: '#5a1b00'
  tertiary-container: '#fc5b00'
  on-tertiary-container: '#4f1700'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#d8e2ff'
  primary-fixed-dim: '#adc6ff'
  on-primary-fixed: '#001a41'
  on-primary-fixed-variant: '#004493'
  secondary-fixed: '#e2e2e2'
  secondary-fixed-dim: '#c6c6c7'
  on-secondary-fixed: '#1a1c1c'
  on-secondary-fixed-variant: '#454747'
  tertiary-fixed: '#ffdbce'
  tertiary-fixed-dim: '#ffb59a'
  on-tertiary-fixed: '#370e00'
  on-tertiary-fixed-variant: '#802a00'
  background: '#0b1326'
  on-background: '#dae2fd'
  surface-variant: '#2d3449'
typography:
  display-metrics:
    fontFamily: Inter
    fontSize: 64px
    fontWeight: '800'
    lineHeight: '1.1'
    letterSpacing: -0.04em
  headline-lg:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
    letterSpacing: -0.02em
  headline-lg-mobile:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '700'
    lineHeight: 32px
  headline-md:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: '600'
    lineHeight: 28px
  body-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  body-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  label-caps:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '700'
    lineHeight: 16px
    letterSpacing: 0.1em
  data-mono:
    fontFamily: JetBrains Mono
    fontSize: 16px
    fontWeight: '500'
    lineHeight: 20px
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  unit: 4px
  gutter: 16px
  margin-mobile: 16px
  margin-desktop: 32px
  container-max: 1440px
---

## Brand & Style
The design system is engineered for elite ski athletes who require split-second data processing in high-glare, high-stakes environments. The brand personality is precise, cold-tuned, and high-performance, evoking the sensation of carving through fresh powder at terminal velocity.

The aesthetic merges **Minimalism** with **Glassmorphism**. It utilizes a "Frosted Ice" UI language—transparent, high-gloss surfaces that provide depth without visual clutter. The interface feels like a high-tech heads-up display (HUD) integrated into a goggles' visor, prioritizing clarity, technical accuracy, and an aggressive, data-driven edge.

## Colors
The palette is rooted in the "Deep Alpine" spectrum to ensure maximum contrast against snow-blindness conditions.

- **Primary (Alpine Blue):** Used for active states, data traces, and primary navigational paths. It represents the sky and ice.
- **Secondary (Snow White):** Used for high-readability typography and essential icons. It provides a crisp, clinical feel.
- **Tertiary (High-Vis Orange):** Reserved strictly for performance alerts, critical gate splits, and peak heart rate zones. It is the "danger and action" color.
- **Neutral (Midnight Void):** A deep, slightly desaturated navy used for backgrounds to allow the glass layers to pop.

## Typography
The system uses **Inter** for its exceptional legibility and neutral, technical character. To reinforce the "high-performance instrument" feel, **JetBrains Mono** is introduced for secondary labels and numeric data readouts, ensuring that gate splits and timestamps are perfectly aligned and easy to scan.

Large display metrics use tight tracking and heavy weights to convey power. Content density is managed through clear typographic hierarchy, ensuring that even under physical duress or high movement, the athlete can extract key metrics at a glance.

## Layout & Spacing
The layout follows a **Fluid Grid** model with a 12-column structure for desktop and a single-column stack for mobile. Spacing is based on a 4px baseline shift to maintain mathematical precision.

Data widgets should be grouped into modular "tiles." On mobile, critical performance metrics (Speed, HR) are pinned to the top 30% of the viewport. On desktop, a dashboard view allows for side-by-side comparison of gate splits and video analysis. Large touch targets are prioritized to accommodate gloved interaction or cold fingers.

## Elevation & Depth
Depth is created through **Glassmorphism** rather than traditional drop shadows. Surfaces use a `backdrop-filter: blur(12px)` and a `background: rgba(255, 255, 255, 0.05)` to simulate frosted ice.

1.  **Base Layer:** The Midnight Void background.
2.  **Surface Layer:** Frosted glass tiles with a 1px inner border (Snow White at 10% opacity) to define edges.
3.  **Active Layer:** Elements that require focus use a more opaque glass or a subtle outer glow in Alpine Blue to indicate elevation.
4.  **Floating Elements:** Global actions use a higher blur radius and a 20% white tint to sit "above" the data tiles.

## Shapes
The shape language is **Soft (0.25rem)**. This subtle rounding provides a modern, engineered feel that avoids the "friendliness" of fully rounded corners while escaping the "harshness" of sharp 0px angles. It mimics the precision-machined edges of ski bindings and carbon fiber equipment. 

Interactive elements like buttons and chips follow this consistent 4px radius, while larger data containers use the `rounded-lg` (8px) token for a more defined structural presence.

## Components
- **Buttons:** Primary buttons are solid Snow White with black text for maximum contrast. Secondary buttons use the "Ice Glass" style with an Alpine Blue stroke.
- **Data Chips:** Small, semi-transparent capsules used for metadata (e.g., "Wind Speed: 12km/h"). They use `label-caps` typography.
- **Metric Cards:** The core component. These feature a `display-metrics` value, a `label-caps` title, and a sparkline graph in the background to show the trend.
- **Gate Split List:** A vertically stacked list where "Current Split" is highlighted with a High-Vis Orange left-border indicator.
- **Gauges:** Circular progress indicators for physical stats (Oxygen, HR) using thin Alpine Blue strokes and glowing caps.
- **Inputs:** Dark, recessed fields with a 1px border that illuminates in Alpine Blue when focused.