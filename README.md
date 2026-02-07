# THERMA - 1D Heat Equation Visualizer

An interactive browser-based visualizer for the 1D heat equation using finite differences (explicit Euler method).

**Live demo:** Open `index.html` in any modern browser.

## Overview

THERMA solves the 1D heat equation:

$$\frac{\partial u}{\partial t} = \alpha \frac{\partial^2 u}{\partial x^2}$$

using an explicit finite difference scheme with automatic stability control (CFL condition).

## Features

- **Interactive drawing:** Click and drag on the plot to draw custom initial temperature profiles
- **8 preset initial conditions:** Sine wave, Gaussian, step function, triangle, two humps, random, square wave, sawtooth
- **Adjustable parameters:** Thermal diffusivity, spatial resolution, segment length, simulation speed, brush size
- **Boundary conditions:** Dirichlet (fixed temperature) and Neumann (insulated/zero flux)
- **Real-time visualization:** Color-coded temperature profile with space-time heatmap
- **Single file:** No dependencies, no build step -- just open in a browser

## Usage

1. Open `index.html` in a web browser
2. Select a preset or draw an initial condition
3. Adjust physics parameters (diffusivity, resolution, length)
4. Set boundary conditions (Dirichlet or Neumann)
5. Click **Play** to run the simulation, or **Step** to advance manually

## Author

Bhaskar Krishnamachari, University of Southern California (USC)

## License

This project is licensed under the [PolyForm Noncommercial License 1.0.0](LICENSE).
