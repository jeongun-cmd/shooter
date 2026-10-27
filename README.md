# OUTBREAK PULSE — Energy Defense Shooter

A single-page HTML Canvas shooter prototype inspired by the forward-facing, lane-based shooting segments of mobile zombie arcade games. It uses original generated artwork and a fictional cleansing pulse instead of firearm imagery.

## Gameplay
- Player moves left/right using arrow keys or A/D, or by dragging across the game area.
- Cyan cleansing pulses fire automatically in a perfectly straight path from the player's current lane.
- Pulses do not home in on enemies. Aim by moving into the same lane as an approaching infected.
- Infected approach along the road in perspective and take two pulse hits to cleanse.
- Each successful cleanse grants 100 points. If an infected reaches the player in the same lane, integrity drops by 20.
- The wave rises after every five cleanses. Higher waves increase enemy speed and spawn rate.
- Includes hit particles, score floaters, damage feedback, pause/resume, and restart.

## Run
Open `index.html` in a modern browser. The assets are stored in `assets/` and no build step or external dependency is needed.