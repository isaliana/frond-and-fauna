# Frond & Fauna — Pool Illustrated

An interactive illustrated swimming pool. Top-down, kidney-bean shaped, surrounded by botanicals. Drop floaties in. Watch the water move.

**[Live demo →](https://isaliana.github.io/frond-and-fauna)**

---

## What it is

A single-file creative experiment: illustrated pool scene with real-time wave physics, draggable floaties, and hand-drawn botanical overlays. No framework, no build step — open `index.html` and it runs.

The pool water uses a 2D Laplacian wave grid with caustic shimmer rendered on a canvas overlay. Ducks are autonomous — they pick targets and swim, leaving wake ripples behind them. Other floaties drift with the current.

---

## Features

- **Live water simulation** — click anywhere in the pool to send ripples; wave energy propagates across the grid frame by frame
- **Floatie palette** — drag beach balls, life rings, rubber ducks (white, yellow, grey), or a corgi on a flamingo float into the pool
- **Autonomous swimmers** — ducks self-propel, steer toward random targets, and re-route when they reach the edge
- **Wake physics** — each swimmer generates ripples proportional to its velocity
- **Botanical frames** — layered SVG greenery composited with `mix-blend-mode: multiply` for a hand-illustrated feel
- **Draggable decorations** — scatter leaves and botanicals around the pool deck from the palette

---

## Assets

```
assets/
  botanicals/    palm leaves, tropical leaves, frame overlays (SVG)
  floaties/      duckie_white, duckie_yellow, duckie_grey, corgi_flamingo (SVG)
```

Floaties are embedded inline as SVG templates on drop, with namespaced IDs so multiple instances don't collide on clipPath/filter definitions.

---

## Running it

```bash
open index.html
```

That's it. No install, no server required.

---

## Status

Work in progress. The pool scene and floatie interactions are complete. Future directions include sound, more floaties, and possibly a day/night cycle.

---

*Made with hand-drawn SVGs and too much love for swimming pools.*
