---
name: Lumina Glass
colors:
  surface: '#f8f9ff'
  surface-dim: '#cbdbf5'
  surface-bright: '#f8f9ff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#eff4ff'
  surface-container: '#e5eeff'
  surface-container-high: '#dce9ff'
  surface-container-highest: '#d3e4fe'
  on-surface: '#0b1c30'
  on-surface-variant: '#464554'
  inverse-surface: '#213145'
  inverse-on-surface: '#eaf1ff'
  outline: '#767586'
  outline-variant: '#c7c4d7'
  surface-tint: '#494bd6'
  primary: '#4648d4'
  on-primary: '#ffffff'
  primary-container: '#6063ee'
  on-primary-container: '#fffbff'
  inverse-primary: '#c0c1ff'
  secondary: '#006c49'
  on-secondary: '#ffffff'
  secondary-container: '#6cf8bb'
  on-secondary-container: '#00714d'
  tertiary: '#825100'
  on-tertiary: '#ffffff'
  tertiary-container: '#a36700'
  on-tertiary-container: '#fffbff'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#e1e0ff'
  primary-fixed-dim: '#c0c1ff'
  on-primary-fixed: '#07006c'
  on-primary-fixed-variant: '#2f2ebe'
  secondary-fixed: '#6ffbbe'
  secondary-fixed-dim: '#4edea3'
  on-secondary-fixed: '#002113'
  on-secondary-fixed-variant: '#005236'
  tertiary-fixed: '#ffddb8'
  tertiary-fixed-dim: '#ffb95f'
  on-tertiary-fixed: '#2a1700'
  on-tertiary-fixed-variant: '#653e00'
  background: '#f8f9ff'
  on-background: '#0b1c30'
  surface-variant: '#d3e4fe'
typography:
  display:
    fontFamily: Inter
    fontSize: 48px
    fontWeight: '700'
    lineHeight: 56px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
    letterSpacing: -0.01em
  headline-lg-mobile:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '700'
    lineHeight: 32px
  headline-md:
    fontFamily: Inter
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
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 40px
  2xl: 64px
  container-max: 1200px
  gutter: 16px
  margin-mobile: 20px
---

## Brand & Style
The design system is centered on emotional clarity and atmospheric immersion. It utilizes a sophisticated **Glassmorphism** style to create a sense of depth and lightness, making the process of mood tracking feel ethereal rather than clinical. 

The aesthetic relies on "frosted" surfaces that sit atop fluid, organic background gradients. These gradients serve as the primary emotional indicator, shifting hues to reflect the user's current state. The interface should feel like a series of translucent panes suspended in a vibrant, color-filled space. High-quality whitespace, crisp line iconography, and subtle motion are essential to maintaining a premium, modern feel that reduces cognitive load and encourages daily reflection.

## Colors
The color palette is functional and emotive. While the **Indigo** primary color defines the brand's core actions and navigation, the system relies heavily on semantic color states to communicate mood:

- **Primary (Indigo):** Used for navigation, primary calls to action, and the "neutral" brand state.
- **Success (Emerald):** Represents positive, energetic, or "Good" moods.
- **Warning (Amber):** Represents "Neutral," "Contemplative," or "Balanced" states.
- **Danger (Rose):** Represents "Stressed," "Angry," or "Anxious" states.
- **Info (Sky):** Represents "Sad," "Tired," or "Low Energy" states.
- **Neutral (Slate):** Used for text hierarchy and subtle UI borders.

Backgrounds should never be solid. Instead, use a mesh gradient that blends these semantic colors based on the user's input. Surfaces use a semi-transparent white (`rgba(255, 255, 255, 0.4)`) in light mode to achieve the glass effect.

## Typography
This design system uses **Inter** exclusively to maintain a clean, systematic, and highly legible appearance. The typography relies on deliberate weight contrast to establish hierarchy against complex blurred backgrounds.

- **Display & Headlines:** Use Bold (700) or Semi-Bold (600) weights with slight negative letter spacing to feel "tight" and modern.
- **Body Text:** Use Regular (400) weight. Ensure high contrast (Slate-900) to remain readable over semi-transparent glass layers.
- **Labels:** Use Medium (500) or Semi-Bold (600) with increased letter spacing for small metadata and button text to improve scanability.

## Layout & Spacing
The system follows a **Mobile-First** fluid grid. 
- **Mobile:** Single column layout with 20px side margins. Elements are stacked vertically to focus on one mood-entry step at a time.
- **Desktop:** 12-column grid with a maximum container width of 1200px. Content is often centered in "Glass Cards" to maintain the focus on the user's emotional data.
- **Rhythm:** An 8px linear scale is used for all padding and margins to ensure consistent proportions. Use larger gaps (40px+) between major sections to emphasize the "light and airy" feel of the design system.

## Elevation & Depth
Elevation is achieved through physical layering rather than traditional heavy shadows.
- **Glass Surfaces:** Apply `backdrop-filter: blur(12px)` and a background of `white` at 40-60% opacity. 
- **Borders:** Every glass element must have a 1px solid border at 20% opacity (white) to define the edge of the "pane."
- **Shadows:** Use extremely soft, long-range shadows (e.g., `0 20px 40px rgba(0,0,0,0.05)`) to lift cards off the background.
- **Z-Index:** Content layers should feel like they are floating at different depths. Use subtle scale transitions (e.g., scale 1.0 to 1.02) on hover to reinforce this physical depth.

## Shapes
The shape language is friendly and organic. 
- **Standard Cards:** Use `rounded-2xl` (1rem / 16px) for the main glass containers.
- **Buttons & Inputs:** Use `rounded-xl` (0.75rem / 12px) to provide a soft but distinct interactive feel.
- **Mood Selection:** Elements like mood emojis or chips should use "Pill" shapes (full border-radius) to feel approachable and tactile.
- **Interactive States:** When active, shapes can slightly expand or increase their blur intensity.

## Components
- **Buttons:** Primary buttons use a solid Indigo gradient. Secondary buttons use the "Glass" style (blur + white tint) with a semi-bold label.
- **Mood Chips:** Large, circular or pill-shaped interactive elements. When selected, they should glow with their respective semantic color (e.g., an Emerald glow for "Happy").
- **Glass Cards:** The primary container for all content. They should have a 1px inner stroke and a soft drop shadow.
- **Input Fields:** Semi-transparent backgrounds with a 1px border that becomes Indigo on focus. Labels sit clearly above the glass field.
- **Progress Indicators:** Soft, rounded bars that use the semantic color of the current mood to show completion of an entry.
- **Icons:** Use Lucide-style line icons with a 1.5px stroke width. Icons should be paired with friendly emojis for mood states to keep the app feeling personal.