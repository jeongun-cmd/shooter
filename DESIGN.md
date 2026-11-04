# OUTBREAK PULSE — Stage System 07 Design Specification

Editable Figma file: https://www.figma.com/design/iQFVQZbVN767rQK2EO62IA

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

## Main progression screen
- Header and field operation title.
- Score, integrity and stage cards; the stage card contains a clear-goal progress bar.
- Portrait game viewport with sector, stage, direct-aim lane guide and lower integrity/shard HUD.
- Sound, manual save/load and pause controls.

## Stage-clear / Ascension Network screen
- Stage-clear title and reward banner.
- Web-like connected skill network, inspired by the supplied diamond-node reference image.
- Six editable upgrade nodes arranged around a central sigil: power, fire rate, vitality, mobility, pierce and barrier.
- Skill detail and available shard balance.
- Next-stage action.

## Progression and balance rules
- Stage 1 goal: 8 cleanses; each subsequent stage adds 3 to the goal.
- Monster rewards and stage-clear rewards increase with stage.
- Stages 2/3/4 introduce runner/tank/wisp types; every fifth stage spawns a brute boss after the final regular kill.
- Enemy integrity, speed and contact damage scale by type and stage.
- Each skill has five levels; its cost scales with level and stage.
- Keyboard and drag share the same maximum movement speed, including the mobility upgrade multiplier.

## Motion and audio
- Screen and HUD use staggered entrance and state-change feedback.
- Survivor movement includes run bob and lean. Enemies have per-archetype idle/sway animation.
- Energy pulses have luminous trails and impact rings; cleanses add particles and floating shard rewards.
- Damage feedback uses brief flash and camera shake; boss and stage-clear moments use stronger but brief effects.
- Figma has a 2-second core/node motion timeline. Game sound is generated through Web Audio and defaults to off until the player enables it.
- `prefers-reduced-motion` disables ambient animation without affecting game logic or information.
## Persistence and monster sprite system
- Save data is versioned in browser `localStorage` and includes stage, clear count, score, shards, integrity and skill levels.
- Autosave runs on a short interval and at important progression transitions; manual Save and Load controls are also provided.
- Dedicated SVG sprite assets are loaded independently for walker, runner, tank, wisp and brute. Canvas adds per-type bob, sway, aura, hit flash and boss effects.
- Save data is browser/device-local; it does not synchronize between devices or browsers.
