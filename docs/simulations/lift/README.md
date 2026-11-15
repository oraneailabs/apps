# Lift Control Lab

An interactive four-stop traction lift (ground plus three floors) simulation in a single HTML file (`index.html`).

- Live 3D shaft (three.js) and machine room with shadows and reflections, driven by the same controller model as the circuit views
- Position displays, call buttons, circuit rungs and demo steps all point at the same 3D parts
- Power circuit, relay control ladder with per-rung notes, inputs and outputs, and a motor and drive simulation
- Door simulation, full demo and door demo
- Explain lift: 17 parts with 3D markers, simple and technical explanations, voice narration, camera motion

## Run

Open `index.html` in a browser. It loads three.js from cdnjs and fonts from Google Fonts, so it needs an internet connection.

```bash
python3 -m http.server 8000
```

Then visit http://localhost:8000/docs/simulations/lift/ from the repository root.
