# 🌌 The Origin Engine

**The Origin Engine** is a self-sustaining, procedurally generated 3D ecosystem built entirely with math and code. It simulates a digital "terrarium" where geography and biology are inextricably linked through real-time feedback loops.



## 🚀 Live Simulation
**[[https://enonymuss-software.github.io/the-origin-engine/]]**

---

## 🛠 Features

### 🌍 Procedural Geography
The terrain is generated using deterministic noise functions. It isn't a static model; it is a mathematical field that can be manipulated in real-time.
* **Dynamic Sea Level:** Shifting the sea level slider recalculates the biomes (Sand, Grass, Snow) on the fly.
* **Synchronized World Rotation:** A unified parent-child coordinate system ensures life-forms stay "locked" to the terrain during rotation.

### 🧬 Biological Logic
The life-forms (represented by glowing particles) are governed by a "Survival of the Fittest" metabolism:
* **Consumption:** Particles graze on green biomass.
* **Resource Depletion:** High-density populations will eat grass faster than it can regrow, turning lush hills into barren dirt.
* **Metabolic States:** * 🟢 **Teal:** Healthy/Grazing.
    * 🌸 **Pink:** High energy (Mating/Reproduction active).
    * 🟡 **Yellow:** Aquatic panic (High-speed search for land).
* **Sustainability:** The engine features a "Goldilocks" equilibrium logic to prevent instant extinction or infinite overpopulation.

## 🎮 Controls
* **World Rotation:** Adjusts the planetary spin speed.
* **Metabolism:** Controls how fast life-forms move and consume energy.
* **Sea Level:** Simulates climate change by flooding or draining the world.
* **Reseed Population:** Injects a fresh generation of ancestors into the system.

---

## 📜 Technical Stack
* **Engine:** [Three.js](https://threejs.org/) (WebGL)
* **Language:** JavaScript / ESM
* **Hosting:** GitHub Pages (Zero-server architecture)

## ⚖️ License
This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

---
*Created as an experiment in emergent complexity and procedural systems.*
