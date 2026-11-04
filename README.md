# OUTBREAK PULSE — Stage System 07

A mobile-first, single-page HTML Canvas arcade shooter built with plain HTML, CSS and JavaScript. The player channels a fictional cleansing pulse from a chest sigil; no handheld equipment is used. Aim by moving between lanes. Pulses travel in straight lines and never home in.

## Main game loop
1. Clear the current stage by cleansing the required number of infected.
2. Earn score and **purification shards** for every monster.
3. Receive a larger stage-clear reward when the stage goal is reached.
4. Spend shards in the web-like Ascension Network skill tree.
5. Enter the next, harder stage with stronger enemies and a larger clear goal.

Stage 1 begins with 8 cleanses. The goal increases by 3 each stage. Every fifth stage ends with an elite brute boss.

## Monster roster
- **Walker** — baseline infected.
- **Runner** — faster and slimmer, introduced from Stage 2.
- **Tank** — heavily armored, slow and durable, introduced from Stage 3.
- **Wisp** — floating, drifting energy-infected, introduced from Stage 4.
- **Brute / Boss** — large elite with high integrity and a large reward, appears on every fifth stage.

Enemy integrity, speed, contact damage, and shard rewards scale upward with stage. Each monster has an animated idle/movement treatment and a distinct visual accent. Brutes get a boss aura and elite health bar.

## Ascension Network skills
Six upgrade nodes are available after each stage:
- **Pulse Power** — +25% pulse damage per level.
- **Fire Rate** — reduces automatic pulse interval by 0.025 seconds per level.
- **Vitality** — +20 maximum integrity and an immediate heal per level.
- **Mobility** — +8% movement speed per level, applied equally to keyboard and drag.
- **Pulse Pierce** — lets each straight pulse hit additional targets.
- **Barrier** — reduces contact damage by 10% per level.

Each node has five levels. Costs grow by skill level and stage. The stage-clear overlay includes the reward summary, editable-feeling diamond nodes, connected web lines, skill descriptions and a next-stage button.

## Controls and audio
- Move left/right with arrow keys or A/D.
- Drag with mouse or touch to set a target lane. Drag and keyboard share the same speed cap; dragging never teleports the survivor.
- Pulses fire automatically in a straight line.
- Pause/resume is available at any time during active combat.
- Sound is off by default. Use **SOUND OFF** to enable synthesized Web Audio effects (pulse, hit, cleanse, damage, upgrade and stage-clear chimes). No external audio files or network requests are required.

## Visual design and motion
- Editable Figma design: https://www.figma.com/design/iQFVQZbVN767rQK2EO62IA
- Figma contains the stage-clear reward screen, six-node skill network and a subtle core/node motion timeline.
- CSS motion: staggered HUD entrance, scanning playfield, status-card and node feedback.
- Canvas motion: survivor run/lean, per-type enemy movement, road flow/dust, glowing pulse trails, orbiting chest-sigil motes, expanding cleanse rings, particles, score floaters and restrained damage feedback.
- Reduced-motion preferences are respected.

## Assets
- `assets/road.jpg` — road background.
- `assets/runner.svg` — open-handed survivor with chest cleansing sigil.
- `assets/zombie.webp` — infected base art used by walker/runner/tank/brute variants.
- Wisp and additional monster accents are drawn with Canvas primitives.

## Run locally
Keep `index.html` beside the `assets/` folder and open `index.html` in a modern browser. No build step or external runtime dependency is needed.