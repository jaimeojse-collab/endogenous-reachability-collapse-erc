# Endogenous Reachability Collapse (ERC)

A minimal dynamical model for loss of recoverability without loss of state space.

## Overview

This repository contains the simulation code supporting the ERC model, where recoverability loss emerges from a dynamically evolving accessibility boundary.

## Model

The system is a slow–fast dynamical model with:

- Fast variables: x(t), y(t)
- Slow internal variable: c(t)

The recoverability boundary is defined as:

a(c) = a₀ − αc

Trajectories that cross the condition:

a(c(t)) − r(t) = 0

fail to return to the base attractor despite its persistence.

## Reproducibility

All figures in the associated preprint can be reproduced directly from the provided notebook.

## Author

Jaime Ojeda  
Independent Researcher

## License

MIT License
