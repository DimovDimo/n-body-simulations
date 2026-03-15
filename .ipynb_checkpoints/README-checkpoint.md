# Multi-Scale N-Body Framework
### An Experimental Journey from Planck Scales to Galactic Dynamics

[![Python 3.8+](https://img.shields.io)](https://www.python.org)
[![License: MIT](https://img.shields.io)](https://opensource.org)
[![Jupyter Lab](https://img.shields.io)](https://jupyter.org)

Created by **Dimo Dimov**

---

## 🌌 Project Overview
This repository contains a comprehensive computational exploration of **orbital mechanics and gravitational chaos**. The project transitions from the fundamental laws of motion to the complex, unpredictable "dance" of multiple celestial bodies interacting in 1D, 2D, and 3D space.

It serves as both a physical simulator and a mathematical laboratory for testing stability, resonance, and deterministic chaos in N-body systems.

## 🚀 Core Objectives
*   **Simulate** stable and chaotic N-body systems using high-precision integrators.
*   **Verify** Keplerian laws and orbital stability across different scales.
*   **Optimize** gravitational force calculations using the **Barnes-Hut algorithm** ($O(N \log N)$).
*   **Visualize** complex trajectories using interactive 3D rendering (Plotly) and smooth animations (Matplotlib).

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
    *   **Chaotic Dynamics:** Demonstration of the **Butterfly Effect** by introducing microscopic perturbations ($10^{-4}$) to initial conditions.
*   **Large Scale N-Body:** Transitioning towards galaxy-scale simulations using hierarchical spatial partitioning.

## 📦 Installation & Usage
To run this project in your local **JupyterLab** environment:

1. **Clone the repository:**
   ```bash
   git clone https://github.com
   cd n-body-simulations
