# OUTBREAK PULSE — Energy Defense Shooter (UI Design Update 05)

This repository's root `index.html` is the current implementation of the Figma-inspired shooter UI. It displays a visible **DESIGN UPDATE 05** badge beside the field-operation heading so you can distinguish it from older downloaded copies.

## Latest UI
- Root page: [index.html](./index.html)
- Editable Figma design: https://www.figma.com/design/iQFVQZbVN767rQK2EO62IA
- UI tokens and layout spec: [DESIGN.md](./DESIGN.md)

## Gameplay
- Move left/right using the arrow keys or A/D.
- Mouse or touch dragging sets a target lane. The player moves toward the target at the **same maximum speed** as keyboard input; dragging does not teleport the player.
- Cyan energy pulses fire automatically in a straight line from the player's current lane. They do not home in on enemies.
- Infected advance along the road, take two pulse hits to cleanse, and award 100 points.
- Contact with an infected in the same lane reduces integrity by 20.
- A new wave starts after five cleanses. The game includes pause/resume and restart.

## Important: open the correct file
Download the latest package linked in the ChatGPT reply and open the package's **root** `index.html`. The first screen should show the **DESIGN UPDATE 05** badge. Old folders and ZIPs already downloaded to your PC do not update when GitHub changes; extract the latest ZIP into a new folder before running it.

## Run
Keep `index.html` beside the `assets/` folder and open it in a modern browser. No build tool or external runtime dependency is required.
