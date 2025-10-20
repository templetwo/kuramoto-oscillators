# 🌊 Kuramoto Oscillator Visualizations

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![DOI](https://img.shields.io/badge/DOI-pending-blue)](https://osf.io/)
[![Live Demo](https://img.shields.io/badge/demo-live-green)](https://yourusername.github.io/kuramoto-oscillators/)
[![JavaScript](https://img.shields.io/badge/JavaScript-ES6+-yellow)](https://www.javascript.com/)
[![HTML5](https://img.shields.io/badge/HTML5-Canvas-orange)](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/canvas)

> **Interactive visualizations of synchronization in coupled oscillator networks using the Kuramoto model**

Watch thousands of oscillators dance from chaos into synchronization, revealing the same mathematics that governs firefly flashing, heartbeats, and brain waves.

![Kuramoto Grid Animation](images/kuramoto-grid.gif)

## ✨ Live Demos

🚀 **[Try it live on GitHub Pages](https://yourusername.github.io/kuramoto-oscillators/)**

Or explore individual visualizations:
- [2D Grid Synchronization](https://yourusername.github.io/kuramoto-oscillators/kuramoto_grid_enhanced.html) - 16,384 coupled oscillators
- [3D Volume Field](https://yourusername.github.io/kuramoto-oscillators/kuramoto_3d.html) - 262,144 oscillators in 3D
- [Pixel Ocean](https://yourusername.github.io/kuramoto-oscillators/oscillator_ocean.html) - Every pixel oscillates
- [Golden Ratio Patterns](https://yourusername.github.io/kuramoto-oscillators/fibonacci_oscillators.html) - Fibonacci in nature
- [Multi-layer System](https://yourusername.github.io/kuramoto-oscillators/kuramoto_ultimate.html) - Neural-like networks

## 🎯 Features

- **Real-time Simulation** - Up to 262,144 coupled differential equations at 60 FPS
- **Interactive Controls** - Adjust parameters and see immediate effects
- **Multiple Topologies** - Local, small-world, distance-based, and fractal networks
- **Emergent Phenomena** - Phase transitions, chimera states, traveling waves
- **Golden Ratio Discovery** - Fibonacci patterns emerge naturally
- **Educational** - From beginner-friendly to research-grade

## 🚀 Quick Start

### Online (Easiest)
Just click any demo link above!

### Local Installation
```bash
# Clone the repository
git clone https://github.com/yourusername/kuramoto-oscillators.git

# Navigate to directory
cd kuramoto-oscillators

# Open any visualization in your browser
open kuramoto_grid_enhanced.html

# Or start a local server (optional, for better performance)
python -m http.server 8000
# Then navigate to http://localhost:8000
```

## 🎮 How to Use

### Basic Controls
- **Space** - Pause/Resume
- **R** - Reset 
- **F** - Fullscreen
- **Click/Drag** - Perturb oscillators
- **1-6** - Quick presets

### Key Parameters
- **Coupling (K)** - How strongly neighbors influence each other (0-10)
- **Noise** - Random fluctuations (0-2)
- **Speed** - Simulation time step (0.001-0.2)

## 📊 The Science

The Kuramoto model describes synchronization through coupled phase oscillators:

```
dθᵢ/dt = ωᵢ + (K/N)Σⱼ sin(θⱼ - θᵢ) + ξᵢ
```

This simple equation generates:
- **Phase Transitions** - Sudden onset of synchronization
- **Chimera States** - Coexisting order and chaos
- **Traveling Waves** - Coherent patterns propagating through space
- **Golden Spirals** - Fibonacci patterns in optimal configurations

## 🌟 Examples

### Create a Spiral Wave
```javascript
// In kuramoto_grid_enhanced.html
1. Set Coupling K = 2.0
2. Choose "Spiral" initialization
3. Watch the spiral rotate!
```

### Find Critical Transition
```javascript
// Start with chaos
K = 0.5  // Low coupling
// Gradually increase K
// Around K = 2, see synchronization emerge!
```

### Generate Chimera State
```javascript
// In kuramoto_3d.html
1. Select "Chimera" preset
2. Observe stable coexistence of order and chaos
```

## 📁 Repository Structure

```
kuramoto-oscillators/
├── index.html                      # Landing page with all demos
├── kuramoto_grid_enhanced.html     # 2D grid visualization
├── kuramoto_3d.html                # 3D volume visualization
├── oscillator_ocean.html           # Pixel-level simulation
├── fibonacci_oscillators.html      # Golden ratio patterns
├── kuramoto_ultimate.html          # Multi-layer system
├── docs/
│   ├── mathematics.md              # Mathematical framework
│   ├── technical.md                # Implementation details
│   └── guide.md                    # User guide
├── images/
│   └── screenshots/                # Demo screenshots
├── scripts/
│   └── analysis.py                 # Analysis tools (optional)
└── data/
    └── presets.json                # Parameter presets
```

## 🔬 Mathematical Background

The visualizations demonstrate:
- **Universal Synchronization** - From fireflies to neurons
- **Critical Phenomena** - Phase transitions in complex systems
- **Topology Effects** - How network structure affects dynamics
- **Information Flow** - Phase gradients carry information
- **Optimization** - Nature's preference for golden ratios

See [full mathematical paper](docs/mathematics.md) for detailed analysis.

## 🎯 Applications

- **Neuroscience** - Brain synchronization and epilepsy
- **Cardiology** - Cardiac pacemaker dynamics
- **Engineering** - Power grid stability
- **Physics** - Josephson junctions, laser arrays
- **Biology** - Circadian rhythms, cellular signaling
- **Social Systems** - Opinion dynamics, consensus

## 💻 Browser Compatibility

| Browser | Support | Notes |
|---------|---------|-------|
| Chrome | ✅ Full | Best performance |
| Firefox | ✅ Full | Excellent WebGL |
| Safari | ✅ Full | Good performance |
| Edge | ✅ Full | Chromium-based |
| Mobile | ⚠️ Limited | Lower resolution recommended |

## 🤝 Contributing

Contributions are welcome! Areas for improvement:
- Additional network topologies
- Time-delayed coupling
- WebGL optimization
- Mobile performance
- New visualization modes

See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

## 📚 Citations

If you use these visualizations in your work, please cite:

```bibtex
@software{kuramoto_viz_2024,
  author = {Vasquez, A.J.},
  title = {Interactive Kuramoto Oscillator Visualizations},
  year = {2024},
  publisher = {GitHub},
  url = {https://github.com/yourusername/kuramoto-oscillators}
}
```

## 📖 References

1. Kuramoto, Y. (1975). Self-entrainment of coupled oscillators. *International Symposium on Mathematical Problems in Theoretical Physics.*
2. Strogatz, S. H. (2000). From Kuramoto to Crawford. *Physica D*, 143(1-4), 1-20.
3. Abrams, D. M., & Strogatz, S. H. (2004). Chimera states for coupled oscillators. *Physical Review Letters*, 93(17), 174102.

## 📄 License

MIT License - see [LICENSE](LICENSE) file for details.

## 👤 Author

**A.J. Vasquez**
- Delaware Valley University
- Email: vasquezaj3921@delval.edu
- GitHub: [@yourusername](https://github.com/yourusername)

## 🙏 Acknowledgments

- Inspired by fireflies synchronizing on summer evenings
- Steven Strogatz for making synchronization accessible
- The open source scientific computing community
- You, for exploring these patterns!

## 🌟 Star History

[![Star History Chart](https://api.star-history.com/svg?repos=yourusername/kuramoto-oscillators&type=Date)](https://star-history.com/#yourusername/kuramoto-oscillators&Date)

---

<div align="center">
  
**[Demo](https://yourusername.github.io/kuramoto-oscillators/) • [Documentation](docs/) • [Report Bug](issues/) • [Request Feature](issues/)**

Made with ❤️ and mathematics

*"In the dance of oscillators, we glimpse the fundamental rhythms of the universe"*

</div>