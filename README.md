# OUTBREAK PULSE — Energy Defense Shooter

A single-page HTML Canvas shooter prototype inspired by forward-facing, lane-based shooting segments of mobile zombie arcade games. The art is custom-made for this project and the player uses a fictional cyan cleansing pulse.

## Gameplay
- Move left/right with arrow keys or A/D.
- Drag with mouse or touch to aim by changing lanes.
- **Drag movement has the same maximum speed as keyboard movement** (1.04 lane units per second); dragging far across the screen no longer teleports the player.
- The cyan pulse fires automatically in a straight line from the player's current lane. It never homes in on enemies.
- Infected approach along the road in perspective and take two pulse hits to cleanse.
- Each successful cleanse grants 100 points. If an infected reaches the player in the same lane, integrity drops by 20.
- The wave rises after every five cleanses. Higher waves increase enemy speed and spawn rate.
- Includes an aiming lane indicator, hit particles, score floaters, damage feedback, pause/resume, wave progression, and restart.

## Visual design
- Editable design specification: [OUTBREAK PULSE — Shooter UI Design](https://www.figma.com/design/iQFVQZbVN767rQK2EO62IA)
- Dark field-console palette with lime/cyan signal accents, readable score/integrity/wave cards, lane targeting, perspective road, and clear control/pause panel.
- Improved infected sprite scale for easier visibility and a grab/grabbing cursor affordance for desktop.

## Run
Open `index.html` in a modern browser. The `assets/` folder contains the road, survivor, and infected art. No build step or external runtime dependency is needed.
