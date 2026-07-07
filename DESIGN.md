---
name: Kinetic Developer Forge
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
  on-surface-variant: '#e8bcb6'
  inverse-surface: '#e5e2e1'
  inverse-on-surface: '#313030'
  outline: '#af8781'
  outline-variant: '#5e3f3a'
  surface-tint: '#ffb4a8'
  primary: '#ffb4a8'
  on-primary: '#690001'
  primary-container: '#ff5542'
  on-primary-container: '#5c0000'
  inverse-primary: '#c00003'
  secondary: '#c8c6c5'
  on-secondary: '#303030'
  secondary-container: '#474746'
  on-secondary-container: '#b7b5b4'
  tertiary: '#91cdff'
  on-tertiary: '#003350'
  tertiary-container: '#2598dd'
  on-tertiary-container: '#002c46'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#ffdad5'
  primary-fixed-dim: '#ffb4a8'
  on-primary-fixed: '#410000'
  on-primary-fixed-variant: '#930001'
  secondary-fixed: '#e5e2e1'
  secondary-fixed-dim: '#c8c6c5'
  on-secondary-fixed: '#1b1b1c'
  on-secondary-fixed-variant: '#474746'
  tertiary-fixed: '#cce5ff'
  tertiary-fixed-dim: '#91cdff'
  on-tertiary-fixed: '#001e31'
  on-tertiary-fixed-variant: '#004b72'
  background: '#131313'
  on-background: '#e5e2e1'
  surface-variant: '#353534'
typography:
  display:
    fontFamily: Inter
    fontSize: 64px
    fontWeight: '800'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '700'
    lineHeight: '1.2'
  headline-lg-mobile:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '700'
    lineHeight: '1.2'
  headline-md:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
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
  label-mono:
    fontFamily: JetBrains Mono
    fontSize: 14px
    fontWeight: '500'
    lineHeight: '1.4'
    letterSpacing: 0.05em
  caption:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '500'
    lineHeight: '1.4'
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  base: 8px
  section-gap: 120px
  section-gap-mobile: 64px
  grid-gutter: 24px
  container-max: 1200px
---

## Brand & Style

This design system is engineered for the high-end software engineer who balances technical rigor with creative execution. The brand personality is **precise, high-performance, and sophisticated**. It targets hiring managers and technical recruiters who value clarity, performance, and attention to detail.

The visual style is **Corporate Modern with a Developer Edge**. It utilizes a "Dark Mode First" philosophy to reduce eye strain and reflect the environment where code is born. The aesthetic focuses on high-contrast accents against deep, monolithic backgrounds, creating a sense of depth and focus. Motion should be purposeful—think "linear" and "snappy" rather than "bouncy," echoing the efficiency of well-optimized algorithms.

## Colors

The palette is anchored by a deep **Charcoal (#121212)** base, providing a "true dark" canvas that makes content pop without the harshness of pure black. 

- **Primary:** The Laravel-inspired **Orange-Red (#FF2D20)** is used sparingly for high-impact actions, status indicators, and focal points.
- **Surface Tiers:** We use **#1E1E1E** for cards and primary containers, and **#252525** for elevated states (hover).
- **Accents:** Success states use a muted emerald, and warnings use a deep amber, but both should be desaturated to keep the primary Orange-Red as the sole vibrant actor.
- **Typography:** Pure white is reserved for headers; all body text should use a slightly dimmed gray to improve long-form legibility.

## Typography

The typography system relies on **Inter** for its neutral, highly legible characteristic that excels in digital interfaces. 

- **Hierarchy:** Use tight line-heights for headlines to create a "locked-in" professional look.
- **Code Integration:** **JetBrains Mono** is introduced for labels, tags, and snippets to reinforce the developer identity. 
- **Scale:** On mobile, display sizes should aggressively scale down while maintaining the heavy weight to preserve brand impact.
- **Contrast:** Utilize font weight (SemiBold vs Regular) rather than just size to differentiate between info-density levels.

## Layout & Spacing

This design system uses a **12-column fixed-width grid** for desktop (1200px max-width) and a fluid single-column layout for mobile.

- **Vertical Rhythm:** Sections are separated by significant whitespace (120px) to give the portfolio a "gallery" feel.
- **Project Grid:** Use a CSS Grid with `repeat(auto-fill, minmax(350px, 1fr))` to ensure cards reflow elegantly without awkward gaps.
- **Margins:** Desktop margins are set at 48px to allow the content room to breathe, while mobile drops to 20px to maximize screen real estate.

## Elevation & Depth

Depth is achieved through **Tonal Layering** rather than traditional shadows. This keeps the UI feeling flat and fast.

- **Level 0 (Background):** #121212.
- **Level 1 (Cards/Sidebar):** #1E1E1E with a subtle 1px solid border (#2D2D2D).
- **Level 2 (Hover/Active):** #252525.
- **Interactive Depth:** When a card is hovered, it should not rise with a shadow; instead, the border color should transition to the Primary Orange-Red (#FF2D20) and the background should subtly lighten.
- **Glassmorphism:** Use a backdrop-blur (20px) on the navigation bar with 80% opacity of the background color to maintain context while scrolling.

## Shapes

The shape language is **Soft (0.25rem / 4px)**. This mimics the "tab" and "window" feel of modern IDEs like VS Code.

- **Buttons & Inputs:** Use the base 4px radius. 
- **Project Cards:** Use `rounded-lg` (8px) to distinguish larger content blocks from small UI elements.
- **Skill Pills:** Use `rounded-full` (pill shape) to provide a organic contrast to the otherwise rigid geometric grid.

## Components

### Project Cards
Cards should feature a 16:9 aspect ratio image at the top, followed by a content area with a title, a brief description in `body-md`, and a row of technology tags using `label-mono`. The entire card is a clickable surface.

### Skill Progress Bars
Instead of thick bars, use "Track and Indicator" styling. The track should be a 4px tall #2D2D2D line. The indicator is the Primary Orange-Red. Include the percentage in `label-mono` positioned above the bar, right-aligned.

### Professional Timeline
A vertical 2px line in #2D2D2D. Each entry features a Primary-colored dot on the line. The date range should use `label-mono` in `text-secondary`, while the job title uses `headline-md`.

### Buttons
- **Primary:** Solid #FF2D20 with White text. No gradients.
- **Secondary:** Transparent background with a 1px #2D2D2D border. On hover, the border becomes #FF2D20.
- **Ghost:** Text-only with an icon. Used for social links (GitHub, LinkedIn).

### Input Fields
Dark backgrounds (#1E1E1E) with a bottom-border only approach or a very subtle full border. Focus state must trigger a 1px Primary color border transition.