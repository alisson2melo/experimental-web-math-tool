# AETHEL — Advanced Experimental Mathematics & Theorem Visualization Lab

> **An interactive, single-file web playground for visualizing, experimenting with, and intuiting complex mathematical theorems across analysis, dynamical chaos, differential geometry, linear algebra, and experimental number theory.**

![HTML5 Canvas & WebGL](https://img.shields.io/badge/Render%20Engine-WebGL%20%2F%20Canvas2D-06b6d4?style=for-the-badge)
![Three.js Engine](https://img.shields.io/badge/3D%20Engine-Three.js%20r128-d946ef?style=for-the-badge)
![Tailwind CSS](https://img.shields.io/badge/Styling-Tailwind%20CSS-10b981?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-amberAccent?style=for-the-badge)

---

## 🔬 Overview

**AETHEL Math Lab** is an interactive mathematical exploration suite designed for researchers, educators, students, and computational math enthusiasts. It transforms abstract theoretical constructs—such as non-linear attractor dynamics, complex domain colorings, and differential manifolds—into real-time visual sandbox environments.

Built using native modern web technologies (HTML5 Canvas, WebGL/Three.js, Tailwind CSS), AETHEL runs entirely in the browser with **zero external dependencies or build steps required**.

---

## ✨ Features & Research Modules

AETHEL is organized into **five distinct theoretical research domains**:

### 1. 🌊 Complex Analysis & Domain Coloring
* **Phase Portraits:** Maps phase angles to continuous HSL colors and modulus values to visual intensity.
* **Logarithmic Modulus Gridlines:** Visualizes level sets and complex contours.
* **Function Sandbox:**
  * Riemann Zeta Polynomial Approximations ($\sum_{n=1}^N \frac{1}{n^z}$)
  * Complex Exponentials ($e^z$)
  * Complex Trigonometric Functions ($\sin z$)
  * Polynomial Mappings ($z^n + c$)

### 2. 🌀 Dynamical Systems & Chaos
* **3D Strange Attractors:** Live Runge-Kutta 4th Order ($\text{RK}4$) numerical integrator for differential flow equations:
  * **Lorenz System:** Rayleigh number ($\rho$), Prandtl number ($\sigma$), and geometry parameter ($\beta$) tuning.
* **2D Non-Linear Maps:**
  * **Clifford Map:** Real-time particle visualizer for trigonometric discrete maps.
* **Fractal Geometry:**
  * **Mandelbrot & Julia Sets:** High-iteration escape-time algorithm with smooth continuous coloring.
  * **Interactive Julia Picker:** Pick any point $c \in \mathbb{C}$ on the Mandelbrot set to render its corresponding Julia set in real-time.

### 3. 🍩 Differential Geometry & Curved Spaces
* **Interactive 3D Manifolds:** Rendered with vertex shading calibrated for topological invariants:
  * **Torus** (Genus-1 compact surface)
  * **Pseudosphere / Tractroid** (Constant negative Gaussian curvature $K = -1$)
  * **Möbius Strip** (Non-orientable single-sided surface)
  * **Enneper Surface** (Minimal surface where mean curvature $H = 0$)
  * **Hyperbolic Saddle Point**
* **Geodesic Trajectories:** Animated numeric solvers tracking geodesic lines along intrinsic metric tensors.

### 4. 📐 Linear Algebra & SVD Transformation
* **Interactive $2 \times 2$ Matrix Sandbox:** Live coefficient manipulation ($a, b, c, d$).
* **Singular Value Decomposition (SVD):** Visualizes unit circle deformation into hyper-ellipses under matrix transformations.
* **Eigenvector & Spectrum Analysis:** Real and complex eigenvalue ($\lambda_1, \lambda_2$) line overlays.
* **Matrix Powers ($A^k$):** Dynamic trajectory warping under matrix exponentiation.

### 5. 🔢 Experimental Number Theory
* **Prime Spirals:**
  * **Ulam Spiral:** Square lattice visualizer highlighting diagonal prime alignments.
  * **Sacks Spiral:** Archimedean spiral tracking prime distribution over continuous curves.
  * **Filter Presets:** Twin primes and Euler's quadratic polynomial prime generators ($n^2 + n + 41$).
* **Collatz Conjecture ($3n+1$ Orbit Tree):** Interactive stopping-time tree branch generator and altitude tracker.

---

## 🚀 Quick Start

### Option 1: Direct File Launch (No Server Needed)
1. Clone or download the repository:
   ```bash
   git clone https://github.com/your-username/aethel-math-lab.git
   cd aethel-math-lab
   ```
2. Open `math_lab.html` in any standard web browser (Chrome, Firefox, Safari, Edge).

### Option 2: Local HTTP Server (Optional)
```bash
npx serve .
# Or using Python 3
python -m http.server 8000
```
Navigate to `http://localhost:8000/math_lab.html`.

---

## 🛠️ Built With

* **Rendering Engine:** Native 2D Canvas API (Fast ImageData manipulation for domain coloring & fractals)
* **3D Engine:** [Three.js (r128)](https://threejs.org/) + OrbitControls
* **Styling:** [Tailwind CSS v3](https://tailwindcss.com/)
* **Icons:** [Lucide Icons](https://lucide.dev/)
* **Typesetting:** [MathJax v3](https://www.mathjax.org/)

---

## 📚 Theorem Presets Included

The built-in **Theorem Preset Selector** lets you jump straight to historic mathematical phenomena:
* **Riemann Zeta Polynomial Truncation:** Observe pole formation along the critical strip.
* **Essential Singularity ($e^{1/z}$):** Picard's Great Theorem in action.
* **Lorenz Butterfly Attractor:** Classic chaotic trajectory ($\rho = 28$).
* **Pseudosphere Geodesics:** Intrinsic hyperbolic geometry.
* **Euler's Prime Quadratic:** Visual evidence of $n^2 + n + 41$ prime density.
* **Collatz $n = 27$ Tree:** High-altitude trajectory orbit.

---

## 📄 License

Distributed under the **MIT License**. See `LICENSE` for details.

---

<p center-align="true">
  Made with ❤️ for Mathematics & Visual Computation.
</p>