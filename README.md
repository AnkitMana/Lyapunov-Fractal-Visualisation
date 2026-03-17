# Lyapunov-Fractal-Visualisation

# Lyapunov Stability Mapping: Exploring Non-Linear Attractors

This repository contains a high-performance Python implementation for visualizing **Lyapunov Exponents** in discrete-time trigonometric systems. By mapping the boundary between order and chaos, we reveal complex fractal structures known as "Stability Islands."

## 🚀 Project Overview
The core of this project is the iteration of the map:
$$x_{n+1} = b \sin^2(x_n + r)$$

Using an **$A^6B^6$ periodic sequence**, we alternate the phase shift $r$ between two values ($r_A$ and $r_B$). This 2D parameter space reveals how specific phase combinations can induce stable "Phase-Locking" in a system that is globally chaotic.

## 🛠️ Technical Stack
- **Python**: Core logic and data processing.
- **Numba JIT**: Used for **machine-code acceleration** and **parallelized execution**, reducing render times from minutes to seconds.
- **Matplotlib**: Advanced data visualization and custom colormap normalization ($v_{max}$ clipping).

## 📈 Evolution of the Results
The following gallery demonstrates the progression from 1D parameter landscapes to high-resolution 2D attractors.

### 1. The 1D Landscape (Initial Test)
*X-axis: Phase ($r$) | Y-axis: Growth ($b$)*
Initial results showed horizontal "stripes," representing 1D bifurcation points without parameter interaction.
![Initial Stripes](images/image_12b067.png)

### 2. High-Resolution "Swirl" Attractor
*Resolution: 2000+ DPI | $b=3.85$*
The final "Macro" render uses tight color clipping to isolate the stable filaments, revealing the organic complexity of the stability node.
![Final Swirl](images/image_1225c1.jpg)

## 📖 How to Run
1. Clone the repository:
   ```bash
   git clone [https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git](https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git)
