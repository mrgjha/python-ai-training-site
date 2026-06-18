---
name: Syntactic Logic
colors:
  surface: '#f9f9ff'
  surface-dim: '#cadaff'
  surface-bright: '#f9f9ff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f1f3ff'
  surface-container: '#e8edff'
  surface-container-high: '#e0e8ff'
  surface-container-highest: '#d7e2ff'
  on-surface: '#041b3c'
  on-surface-variant: '#434654'
  inverse-surface: '#1d3052'
  inverse-on-surface: '#edf0ff'
  outline: '#737685'
  outline-variant: '#c3c6d6'
  surface-tint: '#0c56d0'
  primary: '#003d9b'
  on-primary: '#ffffff'
  primary-container: '#0052cc'
  on-primary-container: '#c4d2ff'
  inverse-primary: '#b2c5ff'
  secondary: '#00687b'
  on-secondary: '#ffffff'
  secondary-container: '#50dcff'
  on-secondary-container: '#005f71'
  tertiary: '#5e3c00'
  on-tertiary: '#ffffff'
  tertiary-container: '#7d5200'
  on-tertiary-container: '#ffca81'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#dae2ff'
  primary-fixed-dim: '#b2c5ff'
  on-primary-fixed: '#001848'
  on-primary-fixed-variant: '#0040a2'
  secondary-fixed: '#afecff'
  secondary-fixed-dim: '#48d7f9'
  on-secondary-fixed: '#001f27'
  on-secondary-fixed-variant: '#004e5d'
  tertiary-fixed: '#ffddb3'
  tertiary-fixed-dim: '#ffb950'
  on-tertiary-fixed: '#291800'
  on-tertiary-fixed-variant: '#624000'
  background: '#f9f9ff'
  on-background: '#041b3c'
  surface-variant: '#d7e2ff'
typography:
  display-lg:
    fontFamily: Hanken Grotesk
    fontSize: 48px
    fontWeight: '700'
    lineHeight: 56px
    letterSpacing: -0.02em
  display-lg-mobile:
    fontFamily: Hanken Grotesk
    fontSize: 36px
    fontWeight: '700'
    lineHeight: 44px
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Hanken Grotesk
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
  headline-sm:
    fontFamily: Hanken Grotesk
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 28px
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  label-code:
    fontFamily: JetBrains Mono
    fontSize: 14px
    fontWeight: '500'
    lineHeight: 20px
  label-caps:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '700'
    lineHeight: 16px
    letterSpacing: 0.05em
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  base: 8px
  container-max: 1280px
  gutter: 24px
  margin-mobile: 16px
  margin-desktop: 40px
  section-gap: 80px
---

## Brand & Style

The design system is engineered for professional technical education, specifically tailored for Python development training. The brand personality is authoritative yet accessible, positioning the trainer as an expert mentor who simplifies complex concepts. The target audience includes career switchers, corporate teams, and software engineers seeking to deepen their backend expertise.

The chosen style is **Corporate / Modern** with a focus on high-utility information density. It prioritizes clarity, structural integrity, and a sense of "logical flow" that mirrors the clean syntax of Python itself. The UI utilizes ample whitespace to reduce cognitive load, ensuring that the educational content remains the primary focus.

## Colors

This design system utilizes a "Technical Trust" palette. The **Primary Blue** (#0052CC) is deep and stable, used for core branding, primary actions, and navigational anchors. The **Secondary Cyan** (#00B8D9) acts as a high-energy accent for progress indicators and interactive highlights. A **Tertiary Gold** (#FFAB00) is reserved exclusively for "Success," "Certifications," and "Premium" callouts to provide warmth against the cool palette.

The background is strictly off-white (#F4F5F7) to reduce glare during long reading sessions, while text follows a strict hierarchy of deep navy grays to ensure optimal contrast and readability.

## Typography

The typography strategy leverages **Hanken Grotesk** for headlines to provide a sharp, contemporary edge that feels modern and engineered. **Inter** is used for body copy due to its exceptional legibility in data-heavy environments. 

Unique to this design system is the use of **JetBrains Mono** for labels, metadata, and code snippets. This creates a psychological bridge between the learning material and the actual coding environment, reinforcing the professional trainer context. All uppercase labels should have a slight letter-spacing increase for better scannability.

## Layout & Spacing

The layout follows a **Fixed Grid** model on desktop, centered within a 1280px container to prevent line lengths from becoming unreadable. A 12-column system is used for course dashboards and landing pages, while a specialized 8-column narrow layout is reserved for long-form article and lesson content to maintain focus.

Spacing is governed by a strict 8px base unit. Vertical rhythm is critical: use `section-gap` between major thematic blocks and `base * 3` (24px) for internal component padding. On mobile, margins compress to 16px, and multi-column grids collapse into a single vertical stack.

## Elevation & Depth

This design system employs **Tonal Layers** supplemented by **Low-contrast Outlines**. Rather than aggressive shadows, depth is communicated through subtle shifts in background gray levels (e.g., a white card on a light gray background).

Where elevation is required for interactivity (like a hovered course card), use a single, highly diffused "Ambient Shadow": `0px 4px 20px rgba(23, 43, 77, 0.08)`. This keeps the interface feeling "flat" and professional while providing enough tactile feedback for usability. Surface-to-surface borders should use a 1px solid stroke in a light neutral tint.

## Shapes

The shape language is **Soft** (roundedness level 1). This choice balances the rigidity of technical software with the approachability of an educational platform. Small elements like checkboxes and "tags" use the base 4px radius, while larger containers like course cards and modal windows use the `rounded-lg` 8px radius. This subtle rounding prevents the UI from feeling "sharp" or intimidating to beginners.

## Components

### Buttons
- **Primary:** Solid Primary Blue background, white text, bold weight. No gradient.
- **Secondary:** Transparent background with a 2px Primary Blue border.
- **Ghost:** Primary Blue text with no border, used for less urgent actions like "Cancel" or "View Docs."

### Course Cards
Cards must feature a top-heavy visual hierarchy: a 16:9 aspect ratio image or technical icon, followed by a Title (headline-sm), a short description (body-md), and a footer containing "Duration" and "Level" labels in JetBrains Mono.

### Tables (Schedules)
Tables use a "Clean Row" style. No vertical lines. Headers are in `label-caps` with a subtle gray background. Rows have a 1px bottom border. Hovering over a row applies a very light blue tint (#F0F5FF) to indicate selection.

### Input Fields
Inputs are rectangular with a 1px stroke. When focused, the stroke thickens to 2px in Primary Blue with a soft 4px outer glow of the same color. Placeholder text must be a legible medium gray.

### Progress Indicators
Used for course tracking. These should be 8px tall linear bars using the Secondary Cyan color for the fill and a light neutral for the track.