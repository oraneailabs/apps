# Lift Control Lab

An interactive five-floor traction lift simulation in a single HTML file (`index.html`).

- Live 3D shaft (three.js) and machine room, driven by the same controller model as the circuit views
- Power circuit, relay control ladder with per-rung notes, inputs and outputs, and a motor and drive simulation
- Door simulation, full demo and door demo
- Explain lift: 17 parts with 3D markers, simple and technical explanations, voice narration, camera motion

## Run

Open `index.html` in a browser. It loads three.js from cdnjs and fonts from Google Fonts, so it needs an internet connection.

```bash
python3 -m http.server 8000
```

Then visit http://localhost:8000/apps/simulations/lift/ from the repository root.
