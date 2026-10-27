# OUTBREAK PULSE UI Design Notes

Editable Figma design: https://www.figma.com/design/iQFVQZbVN767rQK2EO62IA

## Tokens
- Background / Base: `#0E130E`
- Surface / Panel: `#171F14`
- Border / Subtle: `#404F30`
- Text / Primary: `#F2E8D1`
- Text / Secondary: `#A8B59C`
- Accent / Lime: `#C7F36B`
- Accent / Cyan: `#73F4EF`
- Status / Warning: `#FFAB50`

## Layout
Mobile-first HUD with a compact title/status header, score/integrity/wave cards, 9:16 gameplay field, lane indicator, objective, and separate movement/pause panel.

## Input balance
Keyboard and drag movement use the same maximum speed: `1.04` lane units per second. Dragging sets a target lane; the player advances toward it at the capped speed rather than teleporting to the pointer.
