# 🌌 The Origin Engine

**The Origin Engine** is a self-sustaining, procedurally generated 3D ecosystem built entirely with math and code. It simulates a digital "terrarium" where geography and biology are inextricably linked through real-time feedback loops.

This project is part of **#BuildForJoy** — a non-commercial hobby experiment for learning, curiosity, and the pure joy of building. There are no paywalls, subscriptions, or premium tiers. Everything is free and open.

## Why I Built This

I wanted to explore how far a browser-only sketch could go when terrain, resources, and life share one mathematical field. No backend, no accounts, no monetization — just WebGL, noise, and feedback loops that feel alive.

### Lessons learned
- Deterministic noise is enough to drive both geography and biome coloring in real time.
- Parent–child transforms keep life-forms locked to a rotating world without physics engines.
- Simple metabolism rules (graze → reproduce → starve) produce surprisingly stable "Goldilocks" populations.
- Shipping a zero-server demo on GitHub Pages keeps the focus on the idea, not infrastructure.

## Live Demo

**[Play Demo](https://enonymuss-software.github.io/the-origin-engine/)** · **[Open Source](https://github.com/enonymuss-software/the-origin-engine)**

---

## Features

All controls and simulation systems are unlocked for everyone.

### Procedural Geography
The terrain is generated using deterministic noise functions. It isn't a static model; it is a mathematical field that can be manipulated in real-time.
* **Dynamic Sea Level:** Shifting the sea level slider recalculates the biomes (Sand, Grass, Snow) on the fly.
* **Synchronized World Rotation:** A unified parent-child coordinate system ensures life-forms stay "locked" to the terrain during rotation.

### Biological Logic
The life-forms (represented by glowing particles) are governed by a "Survival of the Fittest" metabolism:
* **Consumption:** Particles graze on green biomass.
* **Resource Depletion:** High-density populations will eat grass faster than it can regrow, turning lush hills into barren dirt.
* **Metabolic States:**
    * **Teal:** Healthy/Grazing.
    * **Pink:** High energy (Mating/Reproduction active).
    * **Yellow:** Aquatic panic (High-speed search for land).
* **Sustainability:** The engine features a "Goldilocks" equilibrium logic to prevent instant extinction or infinite overpopulation.

## Controls
* **World Rotation:** Adjusts the planetary spin speed.
* **Metabolism:** Controls how fast life-forms move and consume energy.
* **Sea Level:** Simulates climate change by flooding or draining the world.
* **Reseed Population:** Injects a fresh generation of ancestors into the system.

---

## Tech Stack Explored
* **Engine:** [Three.js](https://threejs.org/) (WebGL)
* **Language:** JavaScript / ESM (import maps, no bundler required)
* **Hosting:** GitHub Pages (zero-server architecture)

## Run Locally

No install step and no API keys. Any static file server works.

```bash
# From the repository root (optional local server)
npx --yes serve .
# or
python -m http.server 8000
```

Then open the served URL (or open `index.html` directly in a modern browser). There is no `npm run dev` script — this is a single-page ESM demo.

---

## License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

> This app is a non-commercial hobby experiment provided "AS IS" without warranty of any kind, express or implied. Use at your own risk.

---

*Built for joy, learning, and emergent complexity. #BuildForJoy*
