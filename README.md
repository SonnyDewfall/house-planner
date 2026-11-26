# house-planner

An interactive furniture planner for the house: three tabs (Ground, First, Second floor), rooms drawn to the dimensions on the agent's floor plan, drag-and-drop furniture that snaps to a centimetre grid and to walls/other furniture, live clearance measurements, and named saved versions of the whole layout.

- **Live, shared version:** hosted as a Claude artifact. Everyone it's shared with sees the same layout and saved versions in real time.
- **`planner.html`** is the artifact source (the page body only).
- **`index.html`** is the same app as a standalone page (e.g. for GitHub Pages). Opened outside Claude it stores everything in that browser only, so it isn't shared.

## Notes on the plan geometry

All units are centimetres. The rooms use the dimensions printed on the plan. The hall, landing and stairs are estimated from the drawing, so they're approximate. Chimney breasts and fitted kitchen units are drawn as fixed obstacles.

To change room shapes, edit the `FLOORS` array near the top of the script in `planner.html`, then regenerate `index.html`.
