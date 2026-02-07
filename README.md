# THERMA - Heat Equation Visualizer

An interactive browser-based visualizer for the heat equation in 1D and 2D, using finite differences (explicit Euler method).

**Live demo:** [https://heat-eq.vercel.app](https://heat-eq.vercel.app)

## Overview

THERMA solves the heat equation:

- **1D:** $\frac{\partial u}{\partial t} = \alpha \frac{\partial^2 u}{\partial x^2}$
- **2D:** $\frac{\partial u}{\partial t} = \alpha \nabla^2 u$

using an explicit finite difference scheme with automatic stability control (CFL condition).

## 2D Mode (default)

- **Heat brush:** Click and drag on the 2D surface to paint heat. Hold to accumulate. Right-click to cool.
- **6 presets:** Center hotspot, four corners, ring, cross, random spots, diagonal
- **Adjustable parameters:** Thermal diffusivity, grid resolution (N x N), domain size, brush radius, brush temperature, simulation speed
- **Boundary conditions:** Dirichlet (fixed temperature at edges) and Neumann (insulated/zero flux)
- **Real-time heatmap:** Color-coded 2D temperature field with bilinear interpolation

## 1D Mode

- **Interactive drawing:** Click and drag on the plot to draw custom initial temperature profiles
- **8 presets:** Sine wave, Gaussian, step function, triangle, two humps, random, square wave, sawtooth
- **Adjustable parameters:** Thermal diffusivity, spatial resolution, segment length, simulation speed, brush size
- **Boundary conditions:** Dirichlet (fixed temperature) and Neumann (insulated/zero flux)
- **Real-time visualization:** Color-coded temperature profile with space-time heatmap

## Usage

1. Open `index.html` (2D) or `index1d.html` (1D) in a web browser
2. In 2D: paint heat with the brush; in 1D: draw an initial condition or select a preset
3. Adjust physics parameters (diffusivity, resolution, domain size)
4. Set boundary conditions (Dirichlet or Neumann)
5. Click **Play** to run the simulation, or **Step** to advance manually
6. Use the toggle button in the header to switch between 1D and 2D modes

## Files

| File | Description |
|------|-------------|
| `index.html` | 2D Heat Equation Visualizer (default) |
| `index1d.html` | 1D Heat Equation Visualizer |

No dependencies, no build step -- just open in a browser.

## Author

Bhaskar Krishnamachari, University of Southern California (USC)

## License

This project is licensed under the [PolyForm Noncommercial License 1.0.0](LICENSE).
