# OUTBREAK PULSE — UI & Motion Specification (Motion Update 06)

Editable Figma design: https://www.figma.com/design/iQFVQZbVN767rQK2EO62IA

## Visual tokens
- Background / Base: `#11170F`
- Surface / Panel: `#1C2519`
- Surface / Elevated: `#222D1D`
- Border / Subtle: `#3D4C32`
- Text / Primary: `#F0E7D2`
- Text / Secondary: `#A9B29E`
- Accent / Lime: `#C7F36A`
- Accent / Cyan: `#73F4EF`
- Status / Warning: `#FFB45E`
- Status / Danger: `#FF6E61`

## Screen hierarchy
1. Brand and system-status header.
2. Operation title and short aiming instruction.
3. Score, integrity and wave cards.
4. Portrait gameplay viewport with mission and wave chips.
5. Direct-aim lane indicator.
6. Lower pulse-energy/purified and integrity panels.
7. Separate movement guidance and pause control.

## Motion choreography
- Entrance: header → title → stat cards → viewport → lower controls (staggered, under 750ms).
- Ambient: slow scan light over the playfield, lane beacon glow and pulse-sigil breathing.
- Character: subtle survivor bob and lean; infected idle bob/sway; ground contact shadow breathes.
- Gameplay: straight energy pulses have a shimmering trail; cleanses produce expanding rings, particles and floating score; damage triggers brief panel feedback and restrained screen shake.
- Figma prototype: 2-second motion timeline with editable manual keyframe tracks on survivor, infected, shadow, active lane and energy label.

## Interaction / accessibility
- Keyboard and drag share the same maximum movement speed (1.04 lane units/second). Drag updates a target lane; the survivor approaches it at a capped speed.
- Pulses travel in a straight line and do not home in.
- Reduced-motion preferences disable ambient entrance/scan/bob effects while preserving readable state changes and core gameplay.
- Visible keyboard focus styles are retained.
