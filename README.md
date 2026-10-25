# D2NN: Diffractive Optical Neural Network Simulation

A simulation of light propagating through a diffractive optical system, with a trainable phase mask that learns to route light.

## What I built

**Phase 1: Propagation engine.** Light propagation using the angular spectrum method, implemented in Python/NumPy and checked against known diffraction patterns (circular slit, single slit).

**Phase 2: Learning to route light.** The same propagation in PyTorch, with a learnable phase mask. Two Gaussian beams enter at different positions, and the mask is trained with Adam so that each beam lands in its own output region (top or bottom).

## Result

A single trained phase mask routes both input beams to their correct output regions, with the loss falling to about 0.001.

## Files

- Full report with figures: `Diffractive Optical Computing Simulating Light-Based Neural Network via Free-Space Wave Propogation and Training a single learnable diffractive layer.pdf`
- Code: see the .ipynb notebook in this repo

## Status

Phases 1 and 2 are complete. Further phases are planned.
