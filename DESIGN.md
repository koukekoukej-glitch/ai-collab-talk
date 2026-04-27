---
version: "alpha"
name: "Property Dashboard Interface"
description: "Property Interface Dashboard Section is designed for demonstrating application workflows and interface hierarchy. Key features include clear information density, modular panels, and interface rhythm. It is suitable for product showcases, admin panels, and analytics experiences."
colors:
  primary: "#DBEAFE"
  secondary: "#0F172A"
  tertiary: "#ECFCCB"
  neutral: "#FFFFFF"
  background: "#FFFFFF"
  surface: "#F8FAFC"
  text-primary: "#0F172A"
  text-secondary: "#64748B"
  border: "#F1F5F9"
  accent: "#DBEAFE"
typography:
  display-lg:
    fontFamily: "System Font"
    fontSize: "48px"
    fontWeight: 600
    lineHeight: "48px"
    letterSpacing: "-0.025em"
  body-md:
    fontFamily: "System Font"
    fontSize: "12px"
    fontWeight: 400
    lineHeight: "16px"
  label-md:
    fontFamily: "System Font"
    fontSize: "14px"
    fontWeight: 500
    lineHeight: "20px"
rounded:
  full: "9999px"
spacing:
  base: "4px"
  sm: "1px"
  md: "2px"
  lg: "4px"
  xl: "6px"
  gap: "6px"
  card-padding: "9px"
  section-padding: "24px"
components:
  button-primary:
    backgroundColor: "#FFF1F2"
    textColor: "#E11D48"
    typography: "{typography.label-md}"
    rounded: "{rounded.full}"
    padding: "8px"
  button-link:
    textColor: "{colors.text-secondary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.full}"
    padding: "8px"
  card:
    rounded: "19px"
    padding: "20px"
---

## Overview

The interface follows a refined, high-contrast dashboard aesthetic designed for complex property management. The mood is professional and airy, utilizing a "glass-to-solid" hierarchy to ground data visualizations. Composition relies on a central constrained container (1360px) centered on a subtle, grid-patterned background, creating a floating app-window effect. Depth is expressed through layered surfaces and organic atmospheric blurs, ensuring focus remains on actionable UI elements.

- **Mood:** Preserve a interface, follows, refined, high, contrast, dashboard tone rather than defaulting to a generic SaaS look.

- **Composition cues:**
  - Layout: Grid
  - Density: Airy
  - Content Width: Full Bleed
  - Framing: Glassy
  - Grid: Strong

## Colors

The color system uses light mode with #DBEAFE as the main accent and #FFFFFF as the neutral foundation.

- **Primary (#DBEAFE):** Main accent and emphasis color.
- **Secondary (#0F172A):** Supporting accent for secondary emphasis.
- **Tertiary (#ECFCCB):** Reserved accent for supporting contrast moments.
- **Neutral (#FFFFFF):** Neutral foundation for backgrounds, surfaces, and supporting chrome.

- **Usage:** Background: #FFFFFF; Surface: #F8FAFC; Text Primary: #0F172A; Text Secondary: #64748B; Border: #F1F5F9; Accent: #DBEAFE

- **Gradients:** bg-gradient-to-br from-white/60 to-white/10, bg-gradient-to-b from-black/40 to-black/20 via-transparent

## Typography

Typography relies on System Font across display, body, and utility text.

- **Display (`display-lg`):** System Font, 48px, weight 600, line-height 48px, letter-spacing -0.025em.
- **Body (`body-md`):** System Font, 12px, weight 400, line-height 16px.
- **Labels (`label-md`):** System Font, 14px, weight 500, line-height 20px.

## Layout

- Grid logic: Employs a 12-column grid system for the main workspace, with an 8/4 split between the primary dashboard and secondary listing sidebar.
- Rhythm: Spacing is consistent and generous, with 32px padding on the main card container and 24px gaps between major sections.
- Alignment: Everything adheres to a soft-cornered grid, with elements grouped into cards that utilize varying padding (16px to 32px) to denote importance.

Treat the page as a grid / full bleed composition, and keep that framing stable when adding or remixing sections.

- **Layout type:** Grid
- **Content width:** Full Bleed
- **Base unit:** 4px
- **Scale:** 1px, 2px, 4px, 6px, 8px, 12px, 16px, 20px
- **Section padding:** 24px, 32px
- **Card padding:** 9px, 16px, 20px, 24px
- **Gaps:** 6px, 8px, 12px, 16px

## Elevation & Depth

- Surface Recipe: Uses white backgrounds with 70-90% opacity over backdrop-blur for floating components.
- Shadows: A singular "light-touch" shadow recipe of 0 20px 60px rgba(0,0,0,0.06) is applied to the main wrapper, with smaller, tighter shadows for cards to define interactive surfaces.
- Border Feel: Thin, 1px borders (slate-100) are essential to maintain legibility against white backgrounds; they provide the "edge" that prevents glass elements from dissolving into the page.

- Radius Hierarchy: Employs a consistent 24px radius for primary dashboard cards and 32px for the main wrapper. 
- Silhouette Discipline: All interactive controls, including nav chips and search bars, utilize full-pill (rounded-full) geometry to provide a soft, approachable contrast to the angular grid structure.
- Icons: Use consistent stroke-width (1.5) and simplified line-art geometry, ensuring they remain legible at small scales.

- Nav Chips: Segmented controls utilizing active-state backgrounds (rose-50) and distinct text colors to provide immediate feedback on active views.
- Data Cards: Feature border-gradient techniques (bg-gradient-to-br from-white/60 to-white/10) to create a premium, "beveled" feel for glass-morphism.
- Form Inputs: Bordered-full inputs with subtle shadow-focus rings (ring-rose-500/20) that maintain the interface's soft aesthetic while signaling focus states.
- Status Badges: Small, circular indicators (e.g., notification dots, percentage labels) to draw the eye toward critical updates without overwhelming the UI.

Surfaces should read as glass first, with borders, shadows, and blur only reinforcing that material choice.

- **Surface style:** Glass
- **Borders:** 1px #F1F5F9; 2px #FFFFFF; 1px #DBEAFE
- **Shadows:** rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.05) 0px 1px 2px 0px; rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.1) 0px 10px 15px -3px, rgba(0, 0, 0, 0.1) 0px 4px 6px -4px; rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.06) 0px 20px 60px 0px
- **Blur:** 12px, 8px

### Techniques
- **Gradient border shell:** Use a thin gradient border shell around the main card. Wrap the surface in an outer shell with 1px padding and a 20px radius. Drive the shell with linear-gradient(to right bottom, rgba(255, 255, 255, 0.6), rgba(255, 255, 255, 0.1)) so the edge reads like premium depth instead of a flat stroke. Keep the actual stroke understated so the gradient shell remains the hero edge treatment. Inset the real content surface inside the wrapper with a slightly smaller radius so the gradient only appears as a hairline frame.

## Shapes

Shapes rely on a tight radius system anchored by 12px and scaled across cards, buttons, and supporting surfaces. Icon geometry should stay compatible with that soft-to-controlled silhouette.

Use the radius family intentionally: larger surfaces can open up, but controls and badges should stay within the same rounded DNA instead of inventing sharper or pill-only exceptions.

- **Corner radii:** 12px, 19px, 20px, 24px, 9999px
- **Icon treatment:** Linear
- **Icon sets:** Solar

## Components

Anchor interactions to the detected button styles. Reuse the existing card surface recipe for content blocks.

### Buttons
- **Primary:** background #FFF1F2, text #E11D48, radius 9999px, padding 8px, border 0px solid rgb(229, 231, 235).
- **Links:** text #64748B, radius 9999px, padding 8px, border 0px solid rgb(229, 231, 235).

### Cards and Surfaces
- **Card surface:** background rgba(255, 255, 255, 0.7), border 0px solid rgb(229, 231, 235), radius 19px, padding 20px, shadow none.
- **Card surface:** background #FFFFFF, border 1px solid rgb(241, 245, 249), radius 24px, padding 24px, shadow rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.05) 0px 1px 2px 0px.
- **Card surface:** background rgba(239, 246, 255, 0.5), border 1px solid rgba(219, 234, 254, 0.5), radius 12px, padding 16px, shadow none.

### Iconography
- **Treatment:** Linear.
- **Sets:** Solar.

## Do's and Don'ts

Use these constraints to keep future generations aligned with the current system instead of drifting into adjacent styles.

### Do
- Do use the primary palette as the main accent for emphasis and action states.
- Do keep spacing aligned to the detected 4px rhythm.
- Do reuse the Glass surface treatment consistently across cards and controls.
- Do keep corner radii within the detected 12px, 19px, 20px, 24px, 9999px family.

### Don't
- Don't introduce extra accent colors outside the core palette roles unless the page needs a new semantic state.
- Don't mix unrelated shadow or blur recipes that break the current depth system.
- Don't exceed the detected expressive motion intensity without a deliberate reason.

## Motion

- Entrance: Elements employ a staggered vertical reveal (y: 20-30px, opacity: 0) on scroll, using a power-out easing curve for a fluid, natural feel. - Hover Effects: Subtle scale transitions (scale-105) are used on imagery to signal interactivity, while button states transition color smoothly (transition-all) to feel responsive. - Timing: Keep entrance animations between 0.6s and 0.8s; faster reveals feel mechanical, while longer durations risk becoming tedious.

**Motion Level:** expressive

**Durations:** 150ms, 700ms, 8000ms, 10000ms, 1000ms

**Easings:** ease, cubic-bezier(0.4, 0, 0.2, 1), ease-in-out

**Hover Patterns:** text, color, shadow

**Scroll Patterns:** gsap-scrolltrigger
