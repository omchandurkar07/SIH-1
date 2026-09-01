---
name: Civic Pulse
colors:
  surface: '#f7f9fb'
  surface-dim: '#d8dadc'
  surface-bright: '#f7f9fb'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f2f4f6'
  surface-container: '#eceef0'
  surface-container-high: '#e6e8ea'
  surface-container-highest: '#e0e3e5'
  on-surface: '#191c1e'
  on-surface-variant: '#45464d'
  inverse-surface: '#2d3133'
  inverse-on-surface: '#eff1f3'
  outline: '#76777d'
  outline-variant: '#c6c6cd'
  surface-tint: '#565e74'
  primary: '#000000'
  on-primary: '#ffffff'
  primary-container: '#131b2e'
  on-primary-container: '#7c839b'
  inverse-primary: '#bec6e0'
  secondary: '#006c49'
  on-secondary: '#ffffff'
  secondary-container: '#6cf8bb'
  on-secondary-container: '#00714d'
  tertiary: '#000000'
  on-tertiary: '#ffffff'
  tertiary-container: '#001a42'
  on-tertiary-container: '#3980f4'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#dae2fd'
  primary-fixed-dim: '#bec6e0'
  on-primary-fixed: '#131b2e'
  on-primary-fixed-variant: '#3f465c'
  secondary-fixed: '#6ffbbe'
  secondary-fixed-dim: '#4edea3'
  on-secondary-fixed: '#002113'
  on-secondary-fixed-variant: '#005236'
  tertiary-fixed: '#d8e2ff'
  tertiary-fixed-dim: '#adc6ff'
  on-tertiary-fixed: '#001a42'
  on-tertiary-fixed-variant: '#004395'
  background: '#f7f9fb'
  on-background: '#191c1e'
  surface-variant: '#e0e3e5'
typography:
  display-lg:
    fontFamily: Plus Jakarta Sans
    fontSize: 48px
    fontWeight: '700'
    lineHeight: 60px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Plus Jakarta Sans
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
    letterSpacing: -0.01em
  headline-lg-mobile:
    fontFamily: Plus Jakarta Sans
    fontSize: 24px
    fontWeight: '700'
    lineHeight: 32px
  headline-md:
    fontFamily: Plus Jakarta Sans
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
  label-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '600'
    lineHeight: 20px
    letterSpacing: 0.05em
  label-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '500'
    lineHeight: 16px
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  unit: 8px
  container-max: 1280px
  gutter: 24px
  margin-mobile: 16px
  margin-desktop: 48px
---

## Brand & Style

The design system is rooted in the concept of "Structural Clarity." It serves a civic-tech ecosystem where reliability, transparency, and impact are paramount. The visual language avoids the frenetic energy of social media in favor of a **Corporate Modern** aesthetic that leans into **Minimalism**.

The brand personality is authoritative yet accessible—a platform that feels like an official but modern utility. The interface utilizes generous whitespace to reduce cognitive load when navigating complex community issues, ensuring the user feels a sense of calm and order. The emotional response should be one of "Agency": the belief that reporting a problem will lead to a structured, visible resolution.

## Colors

This color palette is designed for high legibility and trust.

- **Primary (Deep Navy):** Used for typography, navigation bars, and primary buttons to convey authority.
- **Secondary (Emerald Green):** Reserved for "Solved" states, positive progress indicators, and success actions.
- **Tertiary (Subtle Blue):** Used for secondary interactive elements, links, and informational tags to differentiate from the primary brand color.
- **Neutral (Soft Grays):** A cool-toned gray scale used for subtle containment and background layering.

**Accessibility Note:** All interactive states must maintain a minimum contrast ratio of 4.5:1 against their background. Status indicators should not rely on color alone; always pair Emerald Green with a check icon or "Solved" text label.

## Typography

The system utilizes a dual-font strategy. **Plus Jakarta Sans** provides a modern, slightly friendly geometric touch for headings, while **Inter** is used for body and data-heavy content due to its exceptional legibility and systematic feel.

For mobile layouts, headline sizes scale down significantly to ensure information density remains high without sacrificing clarity. Use the `label-md` role specifically for category tags and status chips to distinguish them from standard body copy.

## Layout & Spacing

The design system employs a **Fluid Grid** model with a maximum container width to prevent line lengths from becoming unreadable on ultra-wide monitors.

- **Grid:** 12-column grid for desktop, 4-column for mobile.
- **Rhythm:** An 8px linear scale (8, 16, 24, 32, 48, 64) is used for all padding and margins. 
- **Reflow:** On mobile, side-by-side card layouts collapse into a single vertical stack. Navigation moves from a top-bar to a bottom-tab bar or a simplified hamburger menu to maximize thumb reach for "Report" actions.

## Elevation & Depth

To maintain a professional and clean aesthetic, the design system utilizes **Tonal Layers** supplemented by **Low-contrast Outlines**.

- **Surface Levels:** The base background is `$neutral-50` (#F8FAFC). Cards and primary containers sit on top in pure White (#FFFFFF).
- **Outlines:** Use a 1px border (#E2E8F0) for all cards and input fields to define boundaries without heavy shadows.
- **Shadows:** Use a single "Soft Lift" shadow for interactive elements like hover states or modals: `0px 4px 12px rgba(15, 23, 42, 0.08)`. This keeps the UI feeling light and avoids a "muddy" appearance.

## Shapes

The shape language is **Soft** and systematic. A standard 0.25rem (4px) radius is applied to small components like checkboxes and small buttons, while a 0.5rem (8px) radius is used for cards and main containers. This balance of sharp precision and slight rounding creates an atmosphere of professional modernism—approachable but disciplined.

## Components

### Problem Cards
Cards are the primary data vehicle. They feature a white background, a 1px border (#E2E8F0), and a 24px internal padding. 
- **Header:** Contains the Status Chip (e.g., "Reported" in Blue, "In Progress" in Amber, "Solved" in Emerald).
- **Body:** Title in `headline-md`, followed by a truncated description in `body-md`.
- **Footer:** Action area with "I'm Affected" (Secondary Button) and "View Details" (Text Link).

### Buttons
- **Primary:** Solid Deep Navy with white text. High contrast for "Report a Problem."
- **Secondary:** Outlined Deep Navy or Subtle Blue. Used for "I'm Affected" or "Follow Update."
- **Ghost:** No background/border, used for "Cancel" or "Go Back" actions.

### Inputs & Forms
Form fields use a 1px border. When focused, the border transitions to Subtle Blue with a 2px outer "halo" of the same color at 20% opacity. Labels must be visible above the field at all times (no disappearing placeholders).

### Status Indicators
Status is communicated through a "Step-Progress" component for reports. It uses a vertical or horizontal line connecting nodes:
- **Completed steps:** Solid Emerald Green.
- **Current step:** Blue with a pulsing ring.
- **Pending steps:** Light Gray.

### Dashboards
Use large-format "Stat Widgets" with a heavy focus on the number (Plus Jakarta Sans, Bold) and a small label below. Data visualizations (charts) should use the primary blue and emerald green to denote volume and resolution rates respectively.