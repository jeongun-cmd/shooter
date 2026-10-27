# OUTBREAK PULSE — Energy Defense Shooter

A responsive single-page HTML Canvas shooter inspired by lane-based mobile zombie arcade games. Original artwork, a fictional cyan cleansing pulse, and a mobile-first field-console interface are used.

## Gameplay
- Move left/right with arrow keys or A/D.
- Drag with mouse or touch to change the target lane.
- Keyboard and drag use the same maximum movement speed: 1.04 lane units per second. Dragging sets a target; it never teleports the player.
- Cyan energy pulses fire automatically in a straight line from the player's current lane. They never home in on enemies.
- Infected approach along the road in perspective and take two pulse hits to cleanse.
- Each successful cleanse grants 100 points. Contact with an infected in the same lane reduces integrity by 20.
- A new wave starts after every five cleanses, with faster enemies and a higher spawn rate.
- Includes a live score/integrity/wave HUD, lane-target indicator, lower pulse and integrity panels, hit particles, score floaters, damage feedback, pause/resume, wave progression, and restart.

## UI design
The current HTML/CSS implements the composition from the editable Figma design: a brand/status header, operation title, three compact stat cards, 9:16 gameplay viewport, mission and wave chips, target lane indicator, lower pulse/integrity cards, and separate movement/pause controls.

- Editable design: https://www.figma.com/design/iQFVQZbVN767rQK2EO62IA
- Design tokens and layout notes: [DESIGN.md](./DESIGN.md)

## Run
Open `index.html` in a modern browser. Keep the `assets/` folder beside it. No build tool or external runtime dependency is required.
