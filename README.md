# AI prompting project: The Octagon Portfolio

A portfolio homepage built entirely by prompting an AI coding assistant (Claude Code). The whole screen is a 3D MMA octagon. Two animated fighters spar in the middle, and rotating the ring brings up each portfolio section on one of its eight sides.

## Features

- Three.js scene with a rotatable octagon. Drag, use the arrow keys or click a side tab to switch sections.
- Two rigged fighters run a procedural fight director: punches, slips, weaves under hooks, pull-backs, sidesteps, blocks, partial blocks, counters, low/body/head kicks, teeps, clinch knees, checks and caught kicks. Both use the same defence tables and momentum swings between them, so neither one dominates.
- A three-round fight with a broadcast HUD (round, 3:00 clock, corners). Round 1 builds from cautious circling, Round 3 is the busiest, and fatigue builds up. Between rounds both fighters walk to their corners.
- At the end of Round 1 the red corner lands a right hand as the clock hits 0:00. The blue corner goes down, stays down, then gets up and fights on. After Round 3 a rematch starts without the scripted knockdown.
- Once all 8 sides have been seen, the blue corner is hurt for about 25 seconds.
- Test hooks: `?at=175` starts the fight clock at 175 s; `?sim=30` simulates 30 s and reports strike stats.
- A sold-out arena around the cage: about 2,700 instanced spectators who stand, clap, film and cheer in reaction to the fight, plus photographers, judges, LED ad boards, screens and sweeping lights. Optional crowd sound, off by default.
- Original MMA-inspired styling (black, red and gold). It uses no real league branding.

## Run it

Open `index.html` in a browser, or serve the folder:

```
python -m http.server 8000
```

Then visit http://localhost:8000. The fighter model is embedded in the page, so there is nothing else to load.
