# Galaga — HTML5 Remake

A self-contained arcade reimagining of the classic 1981 **Galaga** space shooter,
built with vanilla JavaScript and the HTML5 Canvas. No build tools, no dependencies,
no server required.

## Play

Open `index.html` in any modern browser, or serve the folder:

```bash
python -m http.server 8000   # then visit http://localhost:8000
```

## Controls

| Key | Action |
|-----|--------|
| `←` / `→` or `A` / `D` | Move |
| `↑` / `W` | Move up (limited) |
| `Space` | Fire |
| `P` | Pause / Resume |

## Features

- **Formation-flying enemies** that sway, then launch arc dive-bombs and climb back to re-form.
- **Two enemy types**: tougher Boss enemies (2 HP, aggressive) and standard Minions.
- **Power-ups** (`W`) that upgrade your weapon — stack up to a 3-way shot.
- **Enemy AI**: enemies track and fire at the player while diving.
- **Progressive levels**: each cleared stage gets faster and more aggressive.
- **Juice**: particle explosions, animated starfield, flickering thrusters, blink-on-respawn invulnerability.
- **Synthesized sound** via the Web Audio API (no audio assets needed).
- **HUD** tracking score, level, and lives.

## How to clear a stage

Destroy **every** enemy on the field. Enemies that recover keep cycling, so clear them all
to advance.

## Files

- `index.html` — layout, HUD, overlay, styling.
- `game.js` — full game engine (input, entities, AI, physics, audio, rendering).

Enjoy, pilot. 🚀
