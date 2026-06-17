---
name: Dynamic Pop
colors:
  surface: '#0e1417'
  surface-dim: '#0e1417'
  surface-bright: '#333a3d'
  surface-container-lowest: '#080f12'
  surface-container-low: '#161d1f'
  surface-container: '#1a2123'
  surface-container-high: '#242b2e'
  surface-container-highest: '#2f3639'
  on-surface: '#dde3e7'
  on-surface-variant: '#bbc9cf'
  inverse-surface: '#dde3e7'
  inverse-on-surface: '#2b3134'
  outline: '#859398'
  outline-variant: '#3c494e'
  surface-tint: '#3cd7ff'
  primary: '#a8e8ff'
  on-primary: '#003642'
  primary-container: '#00d4ff'
  on-primary-container: '#00586b'
  inverse-primary: '#00677e'
  secondary: '#fface8'
  on-secondary: '#5e0053'
  secondary-container: '#ff23e5'
  on-secondary-container: '#520049'
  tertiary: '#ffd9a1'
  on-tertiary: '#432c00'
  tertiary-container: '#feb528'
  on-tertiary-container: '#6c4900'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#b4ebff'
  primary-fixed-dim: '#3cd7ff'
  on-primary-fixed: '#001f27'
  on-primary-fixed-variant: '#004e5f'
  secondary-fixed: '#ffd7f0'
  secondary-fixed-dim: '#fface8'
  on-secondary-fixed: '#3a0033'
  on-secondary-fixed-variant: '#840076'
  tertiary-fixed: '#ffdeae'
  tertiary-fixed-dim: '#ffba3d'
  on-tertiary-fixed: '#281900'
  on-tertiary-fixed-variant: '#604100'
  background: '#0e1417'
  on-background: '#dde3e7'
  surface-variant: '#2f3639'
typography:
  display-xl:
    fontFamily: Anybody
    fontSize: 64px
    fontWeight: '900'
    lineHeight: '1.1'
    letterSpacing: -0.04em
  headline-lg:
    fontFamily: Anybody
    fontSize: 40px
    fontWeight: '800'
    lineHeight: '1.2'
    letterSpacing: -0.02em
  headline-lg-mobile:
    fontFamily: Anybody
    fontSize: 32px
    fontWeight: '800'
    lineHeight: '1.2'
  headline-md:
    fontFamily: Anybody
    fontSize: 24px
    fontWeight: '700'
    lineHeight: '1.3'
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '500'
    lineHeight: '1.6'
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.5'
  label-mono:
    fontFamily: JetBrains Mono
    fontSize: 14px
    fontWeight: '600'
    lineHeight: '1.0'
    letterSpacing: 0.05em
spacing:
  unit: 8px
  container-padding: 32px
  gutter: 24px
  stack-gap: 16px
  bouncy-padding: 24px 32px
---

## Brand & Style
The design system is built on a high-octane aesthetic of **Neo-Brutalism mixed with high-energy digital playfulness**. It targets a productivity-focused audience that thrives on momentum and tactile feedback. The UI should evoke a sense of urgency, excitement, and accomplishment through heavy-handed visual cues and "unapologetic" structural elements.

The style is defined by:
- **High-Contrast Impact:** Utilizing pure blacks and electric neon tones to create immediate visual hierarchy.
- **Structural Rawness:** Exposed thick borders and "hard" shadows that reject the softness of modern SaaS in favor of a more physical, zine-like digital experience.
- **Kinetic Energy:** The interface should feel alive, with every element ready to "pop" or "snap" upon interaction.

## Colors
This design system utilizes a high-voltage, non-gradient palette to maximize legibility and energy.
- **Electric Blue (#00D4FF):** Primary action color and focus state.
- **Neon Pink (#FF00E6):** Secondary highlights and destructive actions.
- **Cyber Lime (#CCFF00):** Success states, accents, and high-priority indicators.
- **Deep Obsidian (#0A0A0A):** The foundation for the entire UI, providing a void-like depth that makes neons pop.
- **Surface Gray (#1A1A1A):** Used for card backgrounds and elevated containers to provide subtle separation from the background.
- **Black (#000000):** Used exclusively for borders and hard shadows to ground the vibrant colors.

## Typography
The typography strategy pairs expressive, variable-width headlines with hyper-functional body text. 
- **Headlines:** Use **Anybody** with a Black (900) or ExtraBold (800) weight. It should feel chunky and take up significant screen real estate.
- **Body:** Use **Inter** for all task descriptions and long-form text to ensure readability against high-contrast backgrounds.
- **System Labels:** Use **JetBrains Mono** for metadata, dates, and status tags to reinforce the "technical/raw" aesthetic of the system.

## Layout & Spacing
The layout follows a **Fluid Neo-Brutalist Grid**. Spacing is intentionally generous to allow the "hard shadows" room to breathe without overlapping adjacent elements.

- **Grid:** A 12-column fluid grid for desktop with 24px gutters. On mobile, transition to a single-column stack with 20px side margins.
- **The "Bouncy" Padding:** Internal padding for cards and containers should be oversized (minimum 24px) to create a sense of airy lightness that contrasts with the heavy borders.
- **Alignment:** Elements should feel "snapped" to the grid. Use strict vertical rhythm based on the 8px base unit.

## Elevation & Depth
This system abandons traditional soft shadows and blurs in favor of **Hard-Edge Depth**.

- **Hard Shadows:** All cards, buttons, and input fields utilize a 4px to 8px offset shadow with 100% opacity, colored pure Black (#000000). The shadow does not blur.
- **Directional Offset:** Shadows always offset to the Bottom-Right (e.g., `4px 4px 0px #000000`).
- **Active State:** On click or press, the element should translate (+4px, +4px) to perfectly cover its own shadow, simulating a physical button being pressed into the surface.

## Shapes
The shape language is **aggressive and sharp**. 
- **Corners:** 0px radius on all primary elements (cards, buttons, inputs). This reinforces the "Brutalist" influence.
- **Borders:** All interactive or containing elements must have a minimum 4px solid Black (#000000) border.
- **Accents:** Only small decorative elements (like status pips or notification badges) may use a circle shape to contrast against the rigid square layout.

## Components
- **Buttons:** Large, sharp rectangles with 4px borders. Use Primary Blue for the background. On hover, the button should "pop" (scale 1.05 and shift shadow). On active, shift -4px diagonally.
- **Task Cards:** Surface Gray background, 4px Black border, 8px Black hard shadow. Use Cyber Lime for the "Complete" checkbox.
- **Inputs:** Stark White background with 4px Black border. Placeholder text in a muted gray. On focus, the border changes to Primary Blue and the shadow increases in size.
- **Chips/Tags:** Use JetBrains Mono text. Small rectangles with 2px borders. Each category should have a distinct solid color (Pink, Lime, or Blue).
- **Motion (Micro-interactions):** 
    - Use "Spring" physics for all transitions (Stiffness: 400, Damping: 15). 
    - When a task is added, it should "scale up" from 0 with an overshoot effect. 
    - Hovering over a list item should cause a slight "jitter" or "lift" to indicate interactivity.
- **Checkboxes:** Large 32px squares. When checked, the Cyber Lime fill should "impact" the square with a fast scale animation.