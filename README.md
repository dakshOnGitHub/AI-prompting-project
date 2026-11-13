# AI prompting project: The Octagon Portfolio

A portfolio homepage built entirely by prompting an AI coding assistant (Claude Code). The whole screen is a 3D MMA octagon. Two animated fighters spar in the middle, and rotating the ring brings up each portfolio section on one of its eight sides.

## Features

- Three.js scene with a rotatable octagon. Drag, use the arrow keys or click a side tab to switch sections.
- Two rigged fighters run a procedural fight director: punches, slips, weaves under hooks, pull-backs, sidesteps, blocks, partial blocks, counters, low/body/head kicks, teeps, clinch knees, checks and caught kicks. Both use the same defence tables and momentum swings between them, so neither one dominates.
- A three-round fight with a broadcast HUD (round, 3:00 clock, corners). Round 1 builds from cautious circling, Round 3 is the busiest, and fatigue builds up. Between rounds both fighters walk to their corners.
- One minute into Round 1 (2:00 on the clock) the red corner lands a right hand. The blue corner goes down, stays down, then gets up, and the round carries on while he fights more carefully. After Round 3 a rematch starts without the scripted knockdown.
- Once all 8 sides have been seen, the blue corner is hurt for about 25 seconds.
- Test hooks: `?at=55` starts the fight clock at 55 s (just before the knockdown); `?sim=30` simulates 30 s and reports strike stats; `?sound` turns sound on at load, and `__sfx.demo()` in the console plays every sound once.
- A sold-out arena around the cage: about 2,700 instanced spectators who stand, clap, film and cheer in reaction to the fight, plus photographers, judges, LED ad boards, screens and sweeping lights.
- Arena sound (off until you switch it on; the choice is remembered for the browser session). Everything is synthesised live with Web Audio, so there are no audio files and no two hits sound the same. It follows the fight: swishes on misses, different impacts for jabs, hooks, body shots, kicks, checks, blocked kicks and knees, footsteps and pivots, breathing that gets heavier as the fighters tire, the odd grunt, and a crowd that murmurs, roars, gasps, whistles and applauds depending on what lands. The knockdown, round bells and the ten-second clapper all have their own sounds, with arena reverb and panning that follows where the action is on screen.
- Original MMA-inspired styling (black, red and gold). It uses no real league branding.

## Run it

Open `index.html` in a browser, or serve the folder:

```
python -m http.server 8000
```

Then visit http://localhost:8000. The fighter model is embedded in the page, so there is nothing else to load.
