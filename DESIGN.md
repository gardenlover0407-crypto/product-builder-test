---
name: Industrial Precision
colors:
  surface: '#f9faf5'
  surface-dim: '#d9dad6'
  surface-bright: '#f9faf5'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f3f4f0'
  surface-container: '#edeeea'
  surface-container-high: '#e8e8e4'
  surface-container-highest: '#e2e3df'
  on-surface: '#1a1c1a'
  on-surface-variant: '#45474d'
  inverse-surface: '#2f312e'
  inverse-on-surface: '#f0f1ed'
  outline: '#75777d'
  outline-variant: '#c5c6cd'
  surface-tint: '#545e76'
  primary: '#051125'
  on-primary: '#ffffff'
  primary-container: '#1b263b'
  on-primary-container: '#828da7'
  inverse-primary: '#bbc6e2'
  secondary: '#a14000'
  on-secondary: '#ffffff'
  secondary-container: '#fe7a34'
  on-secondary-container: '#622400'
  tertiary: '#001224'
  on-tertiary: '#ffffff'
  tertiary-container: '#0a2742'
  on-tertiary-container: '#768fae'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#d7e2ff'
  primary-fixed-dim: '#bbc6e2'
  on-primary-fixed: '#101b30'
  on-primary-fixed-variant: '#3c475d'
  secondary-fixed: '#ffdbcc'
  secondary-fixed-dim: '#ffb694'
  on-secondary-fixed: '#351000'
  on-secondary-fixed-variant: '#7b2f00'
  tertiary-fixed: '#d1e4ff'
  tertiary-fixed-dim: '#afc9ea'
  on-tertiary-fixed: '#001d36'
  on-tertiary-fixed-variant: '#2f4865'
  background: '#f9faf5'
  on-background: '#1a1c1a'
  surface-variant: '#e2e3df'
typography:
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
  body-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  label-caps:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '700'
    lineHeight: 16px
    letterSpacing: 0.05em
  data-mono:
    fontFamily: JetBrains Mono
    fontSize: 13px
    fontWeight: '450'
    lineHeight: 18px
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  base: 4px
  gutter: 16px
  margin-mobile: 16px
  margin-desktop: 32px
  column-gap: 24px
---

## Brand & Style
The design system is engineered for the high-stakes environment of construction project management. It balances industrial ruggedness with the sophisticated precision of modern SaaS. The brand personality is authoritative, reliable, and meticulously organized, designed to instill confidence in project managers, engineers, and site foremen. 

The aesthetic leverages **Modern Corporate** principles with a **Technical/Industrial** edge. It prioritizes clarity and density, ensuring that complex Gantt charts, resource allocations, and safety logs are legible at a glance. Visual weight is used to signify stability, while high-visibility accents reflect the safety-first culture of the construction industry.

## Colors
The palette is rooted in a deep navy blue (**Primary**) which provides a stable, professional foundation. **Safety Orange** is utilized exclusively as a functional highlight for calls-to-action, warnings, and critical path milestones, ensuring high visibility against the cooler background tones.

A spectrum of **Cool Grays** and **Slate Blues** (Tertiary) are used to differentiate UI layers, such as sidebars and data tables. The background remains a very light off-white or light gray to reduce eye strain during long periods of data entry. Success states should use a muted forest green, while error states leverage a sharp crimson, maintaining a disciplined, industry-standard color logic.

## Typography
Typography is treated as a functional tool. **Inter** is the primary typeface for its exceptional legibility in data-heavy interfaces and its neutral, professional character. For technical data, coordinates, and serial numbers, **JetBrains Mono** is introduced to provide a distinct visual "type" for raw data vs. UI labels.

Hierarchy is established through weight and color rather than dramatic size shifts. Use `label-caps` for table headers and section titles to create a structured, "blueprint" feel. Paragraph text should always maintain a line height of at least 1.4x the font size to ensure readability in dense documentation.

## Layout & Spacing
This design system utilizes a **12-column fluid grid** for desktop and a **single-column flow** for mobile. The spacing logic is based on a **4px baseline grid**, ensuring all elements align with mathematical precision.

Layouts should prioritize vertical density to maximize the information visible on screen without scrolling. Use 16px gutters for standard components, but allow for "compact" modes in data grids (8px padding) to accommodate large datasets. Sidebars are fixed at 240px to provide a consistent navigation anchor, while main content areas expand to fill the remaining viewport.

## Elevation & Depth
Depth is conveyed through **Tonal Layers** and **Low-Contrast Outlines**. Instead of heavy shadows, the system uses subtle 1px borders in a slightly darker or lighter shade of the background color to define boundaries.

When elevation is required (e.g., for modals or floating action buttons), use **Ambient Shadows**: short, sharp shadows with low opacity (e.g., `0px 2px 4px rgba(27, 38, 59, 0.08)`). This creates a "sheet of paper on a desk" effect—professional, flat, and grounded. Content sections should use a "Surface" color that is slightly elevated from the "Background" color to create a clear visual stack.

## Shapes
The shape language is **Soft (0.25rem)**. This slight rounding takes the edge off the industrial aesthetic, making the software feel modern and user-friendly without appearing "bubbly" or consumer-grade. 

Interactive elements like buttons and input fields use the base 4px radius. Larger containers, such as project cards or dashboard panels, can use a slightly larger 8px radius (rounded-lg) to distinguish them as structural layout pieces. Icons should be stroke-based with a 2px weight to match the precision of the typography.

## Components

### Buttons
- **Primary:** Solid #1B263B with white text. High-contrast and authoritative.
- **Secondary:** Solid #F3722C with white text. Reserved for the "Primary Action" of a specific workflow (e.g., "Submit Bid", "Approve Schedule").
- **Ghost:** Transparent background with #415A77 borders. Used for secondary navigation or canceling actions.

### Form Inputs
Fields must have a defined 1px border (#E0E1DD) and a distinct focus state using a 2px navy blue outline. Labels should always be visible above the input, never as placeholder text, to maintain accessibility in the field.

### Data Tables
Tables are the core of this system. They should feature "Zebra Striping" using a very faint gray. Headers use the `label-caps` typography style with a subtle bottom border. Vertical borders are omitted to emphasize the horizontal flow of data.

### Status Chips
Use a "pill" shape (rounded-xl) with a low-saturation background and high-saturation text. For example, "In Progress" should be a light blue background with navy text, while "Delayed" uses a pale orange background with safety orange text.

### Gantt Bars
Timeline bars should be flat with no gradients. Use the Primary Navy for standard tasks and Safety Orange for critical path tasks. Dependency lines should be thin 1px slate-gray lines with micro-arrows.