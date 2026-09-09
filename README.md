# Cell Engine

Cell Engine is a browser-based, multi-state cellular automata sandbox built as a single-page app.

## Features

- Customizable grid size, cell size, and edge wrapping
- Multiple built-in presets (Conway's Life, HighLife, Seeds, Brian's Brain, Wireworld, and more)
- Up to 10 editable states with:
  - Per-state birth and survival rules
  - State-targeted neighbor checks (`check state`)
  - Configurable decay transitions
- Interactive painting, random fill, and clear/reset controls
- Live simulation playback with adjustable speed
- Population and entropy charts with stability/oscillation detection
- Rule mutation tools (manual and automatic)
- Rule import/export as JSON
- Heatmap overlay, presentation mode, and WebM recording export

## Quick Start

1. Clone or download this repository.
2. Open `index.html` in a modern browser.
3. Start with a preset or configure custom states and rules.
4. Use **Run**, **Step**, and **Reset** to control the simulation.

No build step or dependencies are required.

## Controls

- **Draw**: click/touch on the board
- **Erase**: right-click or hold **Shift** while drawing
- **Space**: run/pause
- **S**: step one generation (when paused)
- **C**: clear grid
- **Esc**: exit presentation mode

## Rule Notation

- Two-state rules are shown as `B.../S...` (for example `B3/S23`).
- Multi-state rules include per-state rule fragments and total state count (for example `/C4`).

## Browser Support Notes

- Video export depends on `MediaRecorder` and `canvas.captureStream` support.
- If unsupported, recording is disabled with an in-app status message.
