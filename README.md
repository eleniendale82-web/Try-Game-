# Lumen Run

A complete, no-build 2D arcade survival game for modern desktop and mobile browsers. Pilot a courier through the dark, collect luminous cells, dodge hostile shards, and reach extraction.

## Run

Open `index.html` in a modern browser. No package install, server, or external assets are required. For a local server, run `python -m http.server 8000` in this folder and visit `http://localhost:8000`.

## Controls

- **Move:** WASD or arrow keys; on touch screens, use the directional pad.
- **Dash:** Space or the on-screen DASH button. Dash grants a short burst of speed and invulnerability; it recharges in 1.8 seconds.
- **Pause/resume:** Escape or the pause button.

## Objective

Collect at least 12 light cells and stay alive until the 45 second extraction window opens. Enemies spawn faster as time passes. You have three hull points. Cells increase your score, and a local personal best is saved in browser storage. A flight ends at 120 seconds if extraction requirements are unmet.

## Project structure

```
index.html   UI, screen structure, canvas
styles.css   Responsive styling, layout, and UI effects
game.js      Game loop, movement, enemies, pickups, effects, saves, and controls
README.md    Setup and gameplay guide
```

## Features

- Main menu, settings, pause, victory, defeat, restart, and return-to-menu flows.
- Escalating enemy pressure, collision damage, dash cooldown, collectibles, score, sector indicator, and extraction objective.
- Responsive canvas with keyboard and touch controls.
- Procedural neon visuals and synthesized sound effects; no asset downloads.
- Persistent settings and best score via `localStorage`.
- Reduced-motion setting and pause-on-window-blur behavior.

## Future ideas

Add handcrafted sectors, enemy patterns, music tracks, controller support, and optional upgrade choices between flights.
