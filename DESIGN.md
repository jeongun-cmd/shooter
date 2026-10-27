# OUTBREAK PULSE — UI Design Specification (Design Update 05)

Editable Figma design: https://www.figma.com/design/iQFVQZbVN767rQK2EO62IA

The root `index.html` implements this layout. Its visible `DESIGN UPDATE 05` badge identifies the updated version.

## Tokens
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

## Layout
1. Brand and system status.
2. Operation title and brief instruction.
3. Score, integrity, and wave cards.
4. Portrait gameplay viewport with mission and wave chips.
5. Target-lane indicator with LEFT / CENTER / RIGHT labels.
6. Lower energy/purified card and integrity bar.
7. Separate movement guidance and pause control.

## Responsive and interaction rules
- 9:16 game frame, optimized for a 390px mobile viewport without horizontal overflow.
- Keyboard and drag use the same maximum movement speed: 1.04 lane units per second.
- Pointer motion sets the target lane; the player approaches it with a capped speed instead of teleporting.
- Pulses always travel in a straight line and never home in.
- Reduced-motion support and visible keyboard focus styles are retained.