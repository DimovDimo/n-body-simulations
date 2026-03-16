# Multi-Scale N-Body Framework
### An Experimental Journey from Planck Scales to Galactic Dynamics

Created by **[Dimo Dimov](https://github.com/DimovDimo)**

---

![Gource Visualization](README.md%20resources/gource_video.gif)
![Visualizations](README.md%20resources/Visualizations.png)

## 🖥️ Alternative Viewing
The primary project and all its complex calculations are contained within the **`N-body Simulations.ipynb`** file. However, if you experience issues loading interactive visualizations or animations in your browser, please open the **`N-body Simulations.html`** file. This provides a pre-rendered, stable version of the entire notebook for immediate review.

## ⚠️ Important Disclaimer
**Speculative Content and Potential Inaccuracy**

This project is an experimental exploration of N-body systems and **blends established scientific facts with highly speculative models**. Please be advised that:
*   The content is intended for **educational and creative purposes only**.
*   It contains theoretical derivations and implementation logic that may differ from standard academic models.
*   **It must not be taken as absolute scientific truth** or used as a reference for professional astronomical navigation or peer-reviewed research.

## 🌌 Project Overview
This repository contains a comprehensive computational exploration of **orbital mechanics and gravitational chaos**. The project transitions from the fundamental laws of motion to the complex, unpredictable "dance" of multiple celestial bodies interacting in 1D, 2D, and 3D space.

It serves as both a physical simulator and a mathematical laboratory for testing stability, resonance, and deterministic chaos in N-body systems.

## 🔭 Core Objectives
*   **Simulate** stable and chaotic N-body systems using high-precision integrators.
*   **Verify** Keplerian laws and orbital stability across different scales.
*   **Optimize** gravitational force calculations using the **Barnes-Hut algorithm**.
*   **Visualize** complex trajectories using interactive 3D rendering and smooth animations.

## 🛠️ Technical Features
### 1. Physics Engine
*   **Symplectic Integrator:** Uses the **Velocity Verlet** algorithm to ensure long-term energy conservation and numerical stability.
*   **Softening Parameters:** Implements gravitational softening to prevent singularities (infinite forces) during close particle encounters.
*   **Vectorized Computation:** Heavy use of `NumPy` broadcasting for efficient pairwise force calculations.

### 2. Simulation Scenarios
*   **The 2-Body Problem:** Verification of Elliptical, Parabolic, and Hyperbolic orbits.
*   **The 3-Body Problem:**
    *   **Figure-Eight Orbit:** A remarkable periodic solution where three equal masses follow a single path.
    *   **Hierarchical Systems:** Stable Sun-Planet-Moon configurations.
    *   **Chaotic Dynamics:** Demonstration of the **Butterfly Effect** by introducing microscopic perturbations to initial conditions.
*   **Large Scale N-Body:** Transitioning towards galaxy-scale simulations using hierarchical spatial partitioning.

## 📦 Installation & Usage
To run this project in your local **JupyterLab** environment:

**Clone the repository:**
   ```bash
   git clone https://github.com/DimovDimo/n-body-simulations
   ```

## 🚀 Getting Started

To explore the simulations, follow these steps in your environment:

1. **Open** the notebook: `N-body Simulations.ipynb`.
2. **Execute** the cells **sequentially** from top to bottom. This ensures that all physical constants, helper functions, and data structures are correctly initialized.
3. **Wait** for the rendering: Some high-precision 3D animations may take a few moments to process.

> **Alternative Viewing:** The primary project and all its complex calculations are contained within the `N-body Simulations.ipynb` file. However, if you experience issues loading interactive visualizations or animations in your browser, please open the **`N-body Simulations.html`** file. This provides a pre-rendered, stable version of the entire notebook for immediate review.

## 📊 Visualizations
The framework is designed for deep visual analysis and supports multiple rendering styles to enhance the user experience:

*   **Interactive 3D:** Powered by `Plotly`. These environments allow you to **rotate, zoom, and pan** around chaotic trajectories to inspect them from any angle. Hover over bodies to see real-time X, Y, and Z coordinates.
*   **Space Aesthetic:** High-contrast **dark mode** visualizations optimized for stellar dynamics, featuring glow effects for stars and translucent orbital paths.
*   **Mathematical Plots:** Includes **space-time diagrams**, energy conservation graphs, and comparisons of computational scaling.

---

**Created by [Dimo Dimov](https://github.com/DimovDimo)**