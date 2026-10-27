# OUTBREAK PULSE — UI Design Specification

Editable Figma design: https://www.figma.com/design/iQFVQZbVN767rQK2EO62IA

The web implementation in `index.html` now uses this design hierarchy and palette.

## Visual system
- Background / Base: `#0E130E`
- Surface / Panel: `#171F14`
- Surface / Elevated: `#222D1D`
- Border / Subtle: `#404F30`
- Text / Primary: `#F2E8D1`
- Text / Secondary: `#A8B59C`
- Accent / Lime: `#C7F36B`
- Accent / Cyan: `#73F4EF`
- Status / Warning: `#FFAB50`
- Status / Danger: `#FF6E61`

## Screen hierarchy
1. Brand and system-status header.
2. Operation title and brief aim instruction.
3. Three KPI cards: score, integrity and wave.
4. Portrait gameplay viewport with mission chip and wave badge.
5. Target-lane indicator with explicit LEFT / CENTER / RIGHT labels.
6. Lower pulse-energy/purified counter and integrity panel.
7. Separate movement instructions and pause control.

## Responsive and interaction rules
- Mobile-first game frame with a 9:16 aspect ratio and no horizontal overflow at a 390px viewport.
- Keep canvas and HTML HUD layers aligned; do not put gameplay controls over the player sprite.
- Keyboard and drag both cap movement at 1.04 lane units per second. Pointer movement updates a target lane; the player advances toward it at the same speed as A/D.
- Pulses move in straight lines and never home in. Aim by changing the player's lane.
- Keep reduced-motion support and visible keyboard focus styles.
