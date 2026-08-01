---
name: Amour & Ink
colors:
  surface: '#fff8f4'
  surface-dim: '#ebd6c5'
  surface-bright: '#fff8f4'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#fff1e7'
  surface-container: '#ffead9'
  surface-container-high: '#f9e5d3'
  surface-container-highest: '#f4dfcd'
  on-surface: '#241a0f'
  on-surface-variant: '#524251'
  inverse-surface: '#3a2e22'
  inverse-on-surface: '#ffeee0'
  outline: '#847183'
  outline-variant: '#d6c0d3'
  surface-tint: '#a200ba'
  primary: '#9e00b5'
  on-primary: '#ffffff'
  primary-container: '#c028d7'
  on-primary-container: '#fffbff'
  inverse-primary: '#fbabff'
  secondary: '#b61722'
  on-secondary: '#ffffff'
  secondary-container: '#da3437'
  on-secondary-container: '#fffbff'
  tertiary: '#6b38d4'
  on-tertiary: '#ffffff'
  tertiary-container: '#8455ef'
  on-tertiary-container: '#fffbff'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#ffd6fd'
  primary-fixed-dim: '#fbabff'
  on-primary-fixed: '#36003e'
  on-primary-fixed-variant: '#7c008e'
  secondary-fixed: '#ffdad7'
  secondary-fixed-dim: '#ffb3ad'
  on-secondary-fixed: '#410004'
  on-secondary-fixed-variant: '#930013'
  tertiary-fixed: '#e9ddff'
  tertiary-fixed-dim: '#d0bcff'
  on-tertiary-fixed: '#23005c'
  on-tertiary-fixed-variant: '#5516be'
  background: '#fff8f4'
  on-background: '#241a0f'
  surface-variant: '#f4dfcd'
typography:
  display-romantic:
    fontFamily: Bricolage Grotesque
    fontSize: 48px
    fontWeight: '800'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Bricolage Grotesque
    fontSize: 32px
    fontWeight: '700'
    lineHeight: '1.2'
  headline-lg-mobile:
    fontFamily: Bricolage Grotesque
    fontSize: 28px
    fontWeight: '700'
    lineHeight: '1.2'
  body-md:
    fontFamily: Plus Jakarta Sans
    fontSize: 16px
    fontWeight: '500'
    lineHeight: '1.6'
  label-sm:
    fontFamily: Plus Jakarta Sans
    fontSize: 14px
    fontWeight: '700'
    lineHeight: '1'
rounded:
  sm: 0.5rem
  DEFAULT: 1rem
  md: 1.5rem
  lg: 2rem
  xl: 3rem
  full: 9999px
spacing:
  unit: 8px
  card-padding: 2rem
  section-gap: 4rem
  gutter: 1.5rem
---

## Brand & Style
The design system is centered on the emotional resonance of a modern, digital love letter. It blends **Tactile Skeuomorphism** with **Playful Minimalism** to create a premium, polished experience that feels both personal and high-end. 

The aesthetic is "Soft-Digital Romanticism." It uses physical metaphors—like scalloped edges and textured paper—reimagined with digital-first flourishes like neon glows and fluid gradients. The interface should feel warm, inviting, and precious, evoking the excitement of receiving a hand-delivered gift.

## Colors
This design system utilizes a warm, high-chroma palette against a soft, organic neutral base. 
- **Background**: Use the Soft Cream (#FBE6D4) for all page-level backgrounds to ensure a soft, non-clinical feel.
- **Primary**: The Pink-to-Purple gradient is the main driver of action and hierarchy.
- **Accents**: Red and Purple are used strictly for decorative patterns (like envelope lining) and "Love" states.
- **Surface**: Pure White is reserved for the card containers to provide a clean, high-contrast canvas for the playful typography.

## Typography
The typography strategy relies on the tension between the expressive, quirky headlines and the modern, soft-terminal body text.
- **Headlines**: Use `display-romantic` for hero messages. Apply the Primary Gradient as a text-fill and add a subtle `drop-shadow(2px 2px 0px rgba(139, 92, 246, 0.3))` to simulate a layered, sticker-like effect.
- **Body**: `Plus Jakarta Sans` provides an optimistic and legible contrast. Keep line lengths short to mimic the feel of a physical card.

## Layout & Spacing
The layout follows a **Fluid Grid** with generous safe margins to allow "floating" decorative elements to breathe. 
- **Desktop**: 12-column grid, max-width 1200px.
- **Mobile**: 4-column grid.
- **Rhythm**: Use an 8px base unit. Card containers should have a minimum of 32px internal padding to maintain the "premium" feel.
- **Decor**: Floating heart elements should be placed outside the main grid lines, anchored to card corners with `absolute` positioning.

## Elevation & Depth
Depth in this design system is created through **Ambient Shadows** and **Glows** rather than harsh outlines.
- **Cards**: Use a large, diffused shadow (`0 20px 40px -10px rgba(0,0,0,0.05)`) to make the white card appear as if it is hovering over the cream background.
- **Interactions**: Buttons use a colored outer glow (`box-shadow: 0 0 15px rgba(236, 72, 153, 0.4)`) when hovered to simulate a light-emitting neon effect.
- **Layers**: Use z-index layers effectively: 0 for Background, 10 for Shadows/Glows, 20 for the Card, and 30 for Floating Hearts.

## Shapes
The shape language is dominated by the **Pill** and the **Scallop**.
- **The Scallop**: Every main card container must feature a "scalloped" border. This is achieved via a masking property or a repeating background circle pattern on the card edges.
- **Pill-shaped**: All buttons, tags, and input fields must use `rounded-full` (Pill-shaped) styling to maintain the friendly, soft aesthetic.
- **Decorative**: Hearts and Gift Box icons should have rounded corners and no sharp internal angles.

## Components
- **Scalloped Cards**: The primary container. White background, soft drop shadow, and a 12px "bite" radius for the scalloped edge.
- **Action Buttons**: Pill-shaped, gradient-filled, with a transition scale effect (1.05x) on hover. Include a "heartbeat" animation for the primary CTA.
- **Floating Hearts**: SVG elements of varying sizes and opacity. Use a slight `float` animation (Y-axis oscillation) to create a sense of lightness.
- **Envelope Strips**: Use the `accent-stripe` gradient on the top or bottom 16px of a card or as the liner for modal headers.
- **Input Fields**: Soft cream background with a pink focus border and a subtle internal shadow to indicate "pressed" depth.
- **Gift Box Graphics**: Use thick strokes and rounded corners, colored in the primary/secondary palette.