# Simulations

Interactive, single-page simulations. Each one lives in its own folder and runs in the browser with no build step.

```
docs/simulations/
  index.html          catalog page listing every simulation
  README.md           this file
  lift/
    index.html        the simulation (one self-contained page)
    README.md         what it shows and how to run it
  <new-name>/
    index.html
    README.md
```

## Add a simulation

Use the `simulation` skill, or scaffold by hand:

```bash
python3 ~/.claude/skills/simulation/scripts/new_simulation.py <slug> "<Title>" "<one-line description>"
```

The script copies the starter template into `docs/simulations/<slug>/`, writes a README, and adds a card to `index.html` between the `SIMULATIONS:START` and `SIMULATIONS:END` markers. Then build the simulation in that folder, test it, and commit.

## Conventions

- Folder name: lowercase words joined by hyphens (`lift`, `water-pump`).
- One `index.html` per simulation, no build tools. Libraries load from cdnjs.
- Shared design language: Controls and Settings zones, Light and Dark theme, Simple and Technical explanations, optional voice.
- Commit only the new simulation folder and the catalog change.

## Publishing

`docs/` is served by GitHub Pages. A simulation is live at `/simulations/<slug>/` once it is pushed to `main`.
