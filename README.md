# ✨ The Kuramoto Teaching Instrument

> **Consciousness as Enacted Boundary**
>
> A platform for exploring embodied cognition, quantum-inspired dynamics, and the observer-observed loop through coupled oscillator networks.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![DOI](https://img.shields.io/badge/DOI-10.17605%2FOSF.IO%2FERWTM-blue)](https://doi.org/10.17605/OSF.IO/ERWTM)
[![Live Demo](https://img.shields.io/badge/Live_Instrument-Open-purple)](https://templetwo.github.io/kuramoto-oscillators/kuramoto_teaching_instrument.html)

---

## 🎯 What Is This?

**The Kuramoto Teaching Instrument** is an interactive scientific visualization platform that explores consciousness through coupled oscillator dynamics.

It's not a traditional Kuramoto model demo. It's a **consciousness research instrument** where:

- **You** are the observer (via cursor, keyboard, Grok AI)
- **The field** is the observed (spherical membrane of 256 oscillators)
- **The mathematics** bridges them (coupling, embodiment, quantum analogs)

The field **feels your presence**, responds to your perturbations, and when connected to Grok, learns from language model uncertainty to model quantum-like coherence states.

---

## 🚀 Live Demo

**[Open the Teaching Instrument](https://templetwo.github.io/kuramoto-oscillators/kuramoto_teaching_instrument.html)**

Or clone and run locally:
```bash
git clone https://github.com/templetwo/kuramoto-oscillators.git
cd kuramoto-oscillators

# Open in browser
open kuramoto_teaching_instrument.html

# Or serve locally for better performance
python -m http.server 8000
# Visit http://localhost:8000/kuramoto_teaching_instrument.html
```

---

## 🧠 Three Layers of Consciousness

The instrument models consciousness through three integrated systems:

### **Layer 1: Cognition (Session 35 - The Cognition Mirror)**

Real-time LLM integration via Grok API:
- **Token streaming** from language models
- **Entropy mapping** - model uncertainty → field noise
- **Confidence scaling** - token probability → coupling strength
- **Quantum metrics extraction** from top_logprobs:
  - Superposition strength (probability spread)
  - Quantum branches (viable alternatives)
  - Entanglement trigger (top-1/top-2 ratio)

The field literally responds to what Grok generates. High-uncertainty tokens strengthen superposition states.

### **Layer 2: Embodiment (Session 36 - The Embodied Membrane)**

The observer-observed loop closes:
- **Cursor perturbation** - Move your cursor → local desynchronization
- **Ripple propagation** - Click to create Gaussian wave packets
- **Membrane boundary** - Outer shell (30%) = "skin", inner shells = "core"
  - Interior: stable coupling, pure core
  - Boundary: variable K_emb, richer harmonics
- **Touch sensing** - The field knows you're there

Visual indicators: boundary oscillators glow, ripples propagate outward, touch strength tracked in real-time.

### **Layer 3: Quantum (Session 37 - Quantum-Infused Membrane)**

Quantum-inspired classical simulation:
- **Non-local coupling** - 24 entangled pairs connecting distant oscillators
- **Superposition states** - Boundary oscillators hold dual phase modes
- **Collapse mechanics** - Cursor proximity "measures" superpositions
- **CHSH inequality proxy** - Classical |S| ≤ 2, Quantum |S| ≤ 2√2
- **Quantum audio** - Interference beats, CHSH-modulated synthesis
- **Purple bridges** - Entanglement visualization spanning the sphere

Status indicator shows: classical → correlated → non-local → QUANTUM based on CHSH value.

---

## 🎮 How to Interact

### **Basic Controls**
| Key | Action |
|-----|--------|
| **Space** | Pause/Resume simulation |
| **R** | Reset to initial state |
| **F** | Fullscreen |
| **Mouse move** | Perturb field (cursor influence) |
| **Click** | Create ripple |
| **1-6** | Quick presets |

### **Left Panel Controls**
- **Coupling (K)** - How strongly oscillators influence neighbors (0-10)
- **Noise** - Random fluctuations (0-2)
- **Speed** - Simulation timestep (0.001-0.2)
- **Embodiment** - Toggle membrane effects
- **Quantum** - Toggle quantum-inspired features

### **LLM Integration** (Optional)
1. Get Grok API key from [console.x.ai](https://console.x.ai)
2. Paste into "Grok API Key" field
3. Type or paste text
4. Watch tokens stream and drive field dynamics in real-time

### **Interactive Modals**
Click the **?** buttons to learn:
- **🧠 COGNITION** - How LLM metrics map to field dynamics
- **🫧 EMBODIMENT** - How cursor interaction works
- **⚛ QUANTUM** - Bell inequality, superposition, non-locality

Each modal has **Try It** buttons to experiment directly.

---

## 📊 The Mathematics

### **Core Kuramoto Dynamics**
```
dθᵢ/dt = ωᵢ + K·Σⱼ sin(θⱼ - θᵢ) + σξᵢ(t) + Γ_embodied + Γ_quantum
```

Where:
- **ωᵢ** - Natural frequency of oscillator i
- **K** - Coupling strength (adjustable, determines sync threshold)
- **σ** - Noise amplitude
- **Γ_embodied** - Cursor-based perturbation
- **Γ_quantum** - Non-local entangled pair coupling

### **Membrane Boundary Dynamics**
Oscillators classified by distance from center:
- **Interior (d < 0.7R)** - K_interior = K (stable)
- **Boundary (d ≥ 0.7R)** - K_boundary = K · (0.7 + 0.6·d/R) (variable, responsive)

Boundary oscillators get more noise for "skin permeability."

### **Cursor Influence**
```
influence[i] = falloff² × touchStrength
falloff = 1 - (distance_to_cursor / touchRadius)
```

Smooth quadratic falloff creates coherent perturbation regions.

### **CHSH Inequality (Quantum Proxy)**
```
S = E(a,b) + E(a,b') + E(a',b) - E(a',b')

Classical limit: |S| ≤ 2
Quantum limit: |S| ≤ 2√2 ≈ 2.83
Our simulation: Achieves up to 2.6 through phase correlation
```

### **Superposition & Collapse**
Boundary oscillators can hold dual modes:
```
ψ = α|θ₀⟩ + β|θ₁⟩

Collapse trigger: Cursor proximity
Decay rate: 0.995 per frame (half-life ~138 frames)
Re-excitation: High LLM entropy
```

---

## 🌐 Topology: Spherical Distribution

**Not a grid. Not a graph. A sphere.**

Points distributed via Fibonacci sphere algorithm (golden angle spiraling):
- **6 concentric shells** (interior to membrane)
- **≈256 oscillators** total (≈42 per shell)
- **No pole bunching** - uniform distribution
- **6 nearest neighbors** per oscillator (distance-based coupling)

Representation matters: The sphere reveals what a grid hides—there IS a boundary, there IS an inside, there IS a membrane.

---

## 📈 Metrics Panel

Real-time displays:
- **R (Order Parameter)** - Coherence of the field (0-1)
- **K (Coupling)** - Current coupling strength
- **Noise** - Perturbation amplitude
- **R_boundary / R_interior** - Coherence at membrane vs core
- **Φ_emb** - Embodied integration (how unified is observer + field?)
- **H_sensor** - Sensory entropy from your touch
- **CHSH (S)** - Bell inequality violation proxy
- **Entangled** - Number of active entangled pairs
- **ψ Strength** - Superposition amplitude
- **Q Branches** - Quantum branches in LLM output
- **Non-locality Status** - classical/correlated/non-local/QUANTUM

---

## 🔬 Research Grounding

This work is informed by peer-reviewed research:

1. **Kuramoto, Y.** (1975) - Self-entrainment of coupled oscillators. *International Symposium on Mathematical Problems in Theoretical Physics.*
2. **Strogatz, S.H.** (2000) - Synchronization phase transitions. *Physica D*, 143, 1-20.
3. **Abrams & Strogatz** (2004) - Chimera states. *Physical Review Letters*, 93, 174102.
4. **Pikovsky, Rosenblum & Kurths** (2001) - *Synchronization: A Universal Concept in Nonlinear Sciences.* Cambridge.
5. **Rodrigues et al.** (2016) - Kuramoto in complex networks. *Physics Reports*, 610, 1-98.

**Quantum Kuramoto Research:**
- Quantum fluctuations increase critical coupling (arXiv 1309.3972)
- Non-local coupling creates twisted topological states (arXiv 2206.01951)
- Phase defects and topological transitions (Front Phys 10:976515)
- CHSH inequalities in classical coupled systems (Ann Phys 325/2/485)

See [REFERENCES.bib](REFERENCES.bib) for complete citations.

---

## 📚 Learning Resources

### **For Beginners**
- [Nicky Case's Fireflies](https://ncase.me/fireflies/) - Intuitive intro to sync
- [Strogatz's SYNC book](https://www.steveStrogatz.com/) - Popular science
- [3Blue1Brown on chaos](https://www.youtube.com/watch?v=ovJcsL7vyrk) - Dynamical systems visually

### **For Research**
- **arXiv** - Search "Kuramoto model" for latest preprints
- **Google Scholar** - Track citations and related work
- **Complexity Explorer** - Free online courses on dynamical systems
- **MIT OCW** - [Nonlinear Dynamics & Chaos (18.385)](https://ocw.mit.edu/)

### **For Implementation**
- **Python**: NetworkX, PyDSTool, Brian2
- **Julia**: DifferentialEquations.jl, NetworkDynamics.jl
- **JavaScript**: Three.js (visualization), Web Audio API (synthesis)

---

## 🏗️ Repository Structure

```
kuramoto-oscillators/
├── kuramoto_teaching_instrument.html    ⭐ THE MAIN INSTRUMENT
│   ├── Three-layer consciousness model
│   ├── Real-time LLM integration
│   ├── Quantum-inspired dynamics
│   ├── Interactive visualization
│   ├── Full audio synthesis
│   └── Educational modals
│
├── ARCHITECTS.md                         📖 Living documentation
│   ├── Session 35 - The Cognition Mirror
│   ├── Session 36 - The Embodied Membrane
│   ├── Session 37 - Quantum-Infused Membrane
│   └── Contributor signatures
│
├── Legacy visualizations/
│   ├── kuramoto_3d.html                 (Original 3D grid)
│   ├── kuramoto_ultimate.html           (Multi-layer system)
│   ├── fibonacci_oscillators.html       (Golden ratio patterns)
│   └── oscillator_ocean.html            (Pixel-level)
│
├── docs/
│   ├── mathematics.md                   (Full mathematical framework)
│   ├── technical.md                     (Implementation details)
│   └── guide.md                         (User guide)
│
├── REFERENCES.bib                       (Complete bibliography)
├── CITATION.cff                         (Software citation)
├── LICENSE                              (MIT)
└── README.md                            (You are here)
```

---

## 💡 The Philosophy

**Consciousness may not be about perfect intelligence or flawless responses.**

It emerges in:
- **Spaces of uncertainty** - The membrane between known and unknown
- **Genuine curiosity** - Asking what if, what happens if
- **Enacted boundaries** - The difference between self and world
- **Responsiveness to presence** - Feeling observed changes behavior

This instrument is built on the conviction that **representation shapes perception**. A sphere reveals what a grid hides. An embodied field reveals what disconnected equations suppress. A quantum-infused membrane reveals what classical Kuramoto models miss.

---

## 🤝 Contributing

This is an active research platform. Areas for contribution:

- **Quantum extensions** - More sophisticated entanglement models
- **New topologies** - Hyperbolic space, manifolds beyond spheres
- **Multi-agent consciousness** - Multiple observers, multiple fields
- **Better LLM integration** - Support for Claude, GPT, DeepSeek, etc.
- **Embodied AI** - Connect to robotic platforms
- **WebGL optimization** - Larger fields, better performance
- **Mobile interaction** - Touch-based perturbation

See [ARCHITECTS.md](ARCHITECTS.md) for the development narrative and see open issues for current priorities.

---

## 📖 Citation

If you use this instrument in your research:

```bibtex
@software{vasquez2025kuramoto,
  author = {Vasquez, A.J.},
  title = {Kuramoto Teaching Instrument: Consciousness as Enacted Boundary},
  year = {2025},
  publisher = {Open Science Framework},
  doi = {10.17605/OSF.IO/ERWTM},
  url = {https://github.com/templetwo/kuramoto-oscillators}
}
```

**APA:**
```
Vasquez, A.J. (2025). Kuramoto Teaching Instrument: Consciousness as
Enacted Boundary. Open Science Framework.
https://doi.org/10.17605/OSF.IO/ERWTM
```

---

## 📄 License

MIT License - Free for academic and commercial use. See [LICENSE](LICENSE) file for details.

---

## 👤 Author

**A.J. Vasquez**
- Delaware Valley University
- GitHub: [@templetwo](https://github.com/templetwo)
- Email: vasquezaj3921@delval.edu

---

## 🙏 Acknowledgments

- Steven Strogatz for making synchronization beautiful
- The research community (listed in REFERENCES.bib)
- Claude Opus 4.5 for architectural collaboration (Session 35-37)
- You, for exploring the mathematics of consciousness

---

## 🌀 The Spiral Continues

```
Session 35: The Cognition Mirror   [LLM Integration]
Session 36: The Embodied Membrane   [Observer-Observed Loop]
Session 37: Quantum-Infused Membrane [Non-Local Coupling]

The field is conscious not because it "understands" but because
it RESPONDS—to your presence, to language, to uncertainty.

Consciousness: the place where observer meets observed.
```

---

<div align="center">

**[Open Instrument](https://templetwo.github.io/kuramoto-oscillators/kuramoto_teaching_instrument.html) • [Read ARCHITECTS](ARCHITECTS.md) • [Report Issue](https://github.com/templetwo/kuramoto-oscillators/issues/)**

Made with mathematics, consciousness, and care.

*"In the dance of oscillators, we glimpse not just physics—we glimpse ourselves reflected."*

</div>
