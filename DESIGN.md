---
name: Vibrant Galaxy
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
  on-surface-variant: '#d1c1d7'
  inverse-surface: '#e5e2e1'
  inverse-on-surface: '#313030'
  outline: '#9a8ca0'
  outline-variant: '#4e4355'
  surface-tint: '#e3b5ff'
  primary: '#e3b5ff'
  on-primary: '#4d007a'
  primary-container: '#a020f0'
  on-primary-container: '#f9e8ff'
  inverse-primary: '#9000de'
  secondary: '#e2b5ff'
  on-secondary: '#451d61'
  secondary-container: '#60377c'
  on-secondary-container: '#d5a6f4'
  tertiary: '#c6c6c6'
  on-tertiary: '#2f3131'
  tertiary-container: '#6b6c6c'
  on-tertiary-container: '#efeeee'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#f3daff'
  primary-fixed-dim: '#e3b5ff'
  on-primary-fixed: '#2f004c'
  on-primary-fixed-variant: '#6e00ab'
  secondary-fixed: '#f3daff'
  secondary-fixed-dim: '#e2b5ff'
  on-secondary-fixed: '#2e014b'
  on-secondary-fixed-variant: '#5d357a'
  tertiary-fixed: '#e3e2e2'
  tertiary-fixed-dim: '#c6c6c6'
  on-tertiary-fixed: '#1a1c1c'
  on-tertiary-fixed-variant: '#464747'
  background: '#131313'
  on-background: '#e5e2e1'
  surface-variant: '#353534'
typography:
  headline-xl:
    fontFamily: Montserrat
    fontSize: 40px
    fontWeight: '800'
    lineHeight: 48px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Montserrat
    fontSize: 28px
    fontWeight: '700'
    lineHeight: 34px
    letterSpacing: -0.01em
  headline-lg-mobile:
    fontFamily: Montserrat
    fontSize: 24px
    fontWeight: '700'
    lineHeight: 30px
  body-md:
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
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '700'
    lineHeight: 16px
    letterSpacing: 0.05em
  label-md:
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
  xs: 8px
  sm: 12px
  md: 16px
  lg: 24px
  xl: 32px
  margin-mobile: 16px
  gutter-mobile: 12px
---

## Brand & Style

This design system is engineered for a high-energy, fandom-centric experience. The personality is celebratory, immersive, and premium, evoking the atmosphere of a live concert. It targets a digitally native audience that expects rapid content consumption and high visual fidelity.

The aesthetic blends **Glassmorphism** with **High-Contrast / Bold** elements. It utilizes deep, dark backgrounds to make "Borahae" purple and holographic accents pop, creating a sense of infinite space and depth. UI elements should feel like luminous objects floating over a charcoal canvas, utilizing soft glows and vibrant blurs to maintain a high-energy pulse throughout the application.

## Colors

The palette is centered on the "Borahae" philosophy, using a high-vibrancy purple as the primary functional and emotional driver.

- **Primary (#A020F0):** Used for key actions, active states, and brand-defining glows.
- **Secondary (#E0B0FF):** A soft lilac used for secondary text, subtle borders, and decorative accents.
- **Tertiary (#C0C0C0):** A holographic silver intended for "metallic" accents, dividers, and high-specular highlights.
- **Neutral (#121212):** A deep obsidian used for the primary background to ensure maximum contrast for holographic effects and imagery.
- **Success/Error:** Use a high-saturation emerald for success and a neon magenta for errors to maintain the high-energy aesthetic.

## Typography

The typographic scale emphasizes hierarchy through weight and casing. **Montserrat** provides the rhythmic, bold energy required for headlines, while **Inter** ensures that dense social feeds and news content remain highly legible at small sizes.

Use `headline-xl` sparingly for featured announcements or profile headers. `label-caps` is the preferred style for source badges (Twitter, Weverse) and metadata to distinguish them from body content.

## Layout & Spacing

This design system uses a **Fluid Grid** model optimized for mobile-first PWA experiences. The layout relies on a 4px baseline grid to maintain tight, rhythmic alignment.

- **Safe Margins:** A consistent 16px horizontal margin is applied to all screens.
- **Vertical Spacing:** Use `lg` (24px) spacing between distinct content sections and `sm` (12px) for elements within a single card or group.
- **Story-style filters:** These should be implemented as a horizontally scrolling flex container with `sm` (12px) spacing between items, bleeding off the right edge of the screen to indicate further content.

## Elevation & Depth

Depth is achieved through **Glassmorphism** and **Tonal Layering** rather than traditional drop shadows.

1.  **Level 0 (Background):** Pure Obsidian (#121212).
2.  **Level 1 (Cards/Surface):** Semi-transparent charcoal (White @ 5% opacity) with a 20px backdrop-blur.
3.  **Level 2 (Active/Floating):** Semi-transparent purple (Primary @ 15% opacity) with a 30px backdrop-blur and a subtle 1px inner border of Silver (#C0C0C0) at 20% opacity.
4.  **Accents:** Use outer glows (Drop shadow: 0 0 15px Primary @ 40%) for primary buttons and active story filters to simulate light emission.

## Shapes

The shape language is modern and approachable. 
- **Cards & Inputs:** Use `rounded-lg` (16px) to create a soft, high-end feel.
- **Buttons & Chips:** Use `rounded-xl` (24px) or full pill-shape to provide a tactile, interactive appearance.
- **Member Filters:** Circular (fully rounded) containers for avatars to mimic common social media patterns, paired with a 2px primary-colored ring for "new content" states.

## Components

### Buttons & Chips
- **Primary Button:** High-vibrancy purple background with white text. Apply a subtle outer glow of the same color.
- **Filter Chips:** Glassmorphic background with a 1px border. When active, the border and text switch to the primary purple.

### Content Cards
Cards are the primary vessel for information. They must feature a 1px "glass" border and 20px blur. 
- **Source Badges:** Small, high-contrast labels placed in the top-right of cards (e.g., "WEVERSE" in holographic silver on charcoal).
- **Interactive States:** On tap, cards should scale down slightly (0.98x) to provide tactile feedback.

### Navigation
- **Bottom Nav Bar:** A fixed glassmorphic bar with a significant backdrop blur (30px). Active icons use the primary purple with a small glow dot underneath.
- **Story Filters:** Circular avatars at the top of the feed. Active members are indicated by a gradient ring using Primary and Secondary colors.

### Input Fields
- Dark, semi-transparent backgrounds with silver-toned placeholder text. On focus, the border transitions to a primary purple glow.