# Frond & Fauna — Pool Illustrated

An interactive illustrated swimming pool. Top-down, kidney-bean shaped, surrounded by botanicals. Drop floaties in. Watch the water move.

**[Live demo →](https://isaliana.github.io/frond-and-fauna)**

---

## What it is

A single-file creative experiment: illustrated pool scene with real-time wave physics, draggable floaties, and hand-drawn botanical overlays. No framework, no build step — open `index.html` and it runs.

The pool water uses a 2D Laplacian wave grid with Worley-cell caustic shimmer rendered on a canvas overlay. Ducks and a curly little swimming dog are autonomous — they pick targets, paddle toward them, and leave wake ripples behind. Other floaties (beach ball, life ring, corgi on a flamingo float) drift with the current.

---

## Features

- **Live water simulation** — click and hold anywhere in the pool to send rippling rings; wave energy propagates across a grid frame by frame
- **Floatie palette** — drag beach balls, life rings, rubber ducks (white, yellow, grey), a swimming dog, or a corgi on a flamingo float into the pool
- **Autonomous swimmers** — ducks and the dog self-propel, steer toward random targets, and re-route when they reach the edge
- **Wake physics** — each swimmer emits expanding rings proportional to its velocity
- **Animated sub-elements** — duck tails wiggle, dog paws paddle in diagonal pairs, corgi ears flap happily, leaves sway in a soft breeze
- **Botanical frames** — three layered SVG greenery overlays (background + corner + palm-leaf) composited with `mix-blend-mode: multiply` for a hand-illustrated feel
- **Draggable decorations** — scatter tropical leaves and a random sample of 12 botanicals around the pool deck from the palette

---

## Assets

```
assets/
  botanicals/    palm leaves, tropical leaves, frame overlays, 60-cell botanical grid (SVG)
  floaties/      duckie_white, duckie_yellow, duckie_grey, corgi_flamingo (SVG)
```

The swimming dog is drawn entirely inline in `index.html` (no external asset). Floaties are embedded inline as SVG templates and stamped on drop with namespaced IDs so multiple instances don't collide on clipPath/filter definitions.

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
