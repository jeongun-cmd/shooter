# OUTBREAK PULSE — Energy Defense Shooter (Motion Update 06)

A responsive, mobile-first HTML Canvas arcade game. The character channels a fictional cleansing pulse from a chest sigil; no handheld equipment is used. The player aims by moving between lanes, while pulses travel straight and never home in.

## Gameplay
- Move left/right with arrow keys or A/D.
- Drag with mouse or touch to choose a target lane. Keyboard and drag share the same maximum speed (1.04 lane units per second); dragging does not teleport the character.
- The character automatically emits straight-line cleansing pulses from the energy sigil.
- Infected approach along the road in perspective and take two pulse hits to cleanse.
- Each cleanse grants 100 points. Contact in the same lane reduces integrity by 20.
- A new wave starts after five cleanses, with faster infected and a higher spawn rate.
- Includes pause/resume, restart, score and integrity HUD, hit feedback and wave progression.

## Design and motion
- Editable Figma design: https://www.figma.com/design/iQFVQZbVN767rQK2EO62IA
- Figma includes a 2-second motion timeline for the survivor bob, infected idle movement, ground-shadow breathing, lane beacon and pulse-energy label.
- HTML/CSS: staggered screen entry, stat-card reveal, scanning light, lane beacon glow, objective icon breathing, button feedback and value-change animations.
- Canvas: moving road reflectors and dust, survivor run/lean motion, infected bob/sway, glowing pulse trails, orbital chest-sigil motes, expanding cleanse rings, particles, score floaters and damage feedback.
- Reduced-motion preferences are respected.

## Assets
- `assets/road.jpg` — road background
- `assets/runner.svg` — original open-handed survivor with a chest energy sigil
- `assets/zombie.webp` — infected character sprite

## Run
Open `index.html` in a modern browser while keeping the `assets/` folder beside it. No build tools or external runtime libraries are required.
