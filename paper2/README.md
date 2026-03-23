# Paper 2 – Ensemble Reachability Collapse

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.19189310.svg)](https://doi.org/10.5281/zenodo.19189310)

DOI: https://doi.org/10.5281/zenodo.19189310

This document presents the ensemble-level extension of the Endogenous Reachability Collapse (ERC) framework.

While Paper 1 introduces a minimal dynamical system where recoverability becomes inaccessible due to internal constraints, this work explores how that phenomenon manifests across a distribution of initial conditions.

---

## 📌 Core Idea

Instead of focusing on a single trajectory, we analyze the **fraction of initial conditions** that return to the base attractor.

This provides an operational measure of:

- accessibility of recovery
- robustness of the system
- sensitivity to internal constraint levels

---

## 🔍 Key Result

Numerical simulations suggest that:

> As internal constraint increases, the recoverable fraction collapses rapidly.

Importantly:

- The base attractor remains present in the state space  
- Loss of function occurs through **loss of accessibility**, not removal of states  

---

## 📊 Contents

- `ERC-paper-2-ensemble.pdf`  
  Formal description of the model and results  

- `ercm_simulation.ipynb`  
  Reproducible simulations used to generate results  

- `figures/`  
  Visualizations of:
  - contraction of recoverable set  
  - basin maps across constraint levels  
  - recoverable fraction vs constraint  

---

## ⚙️ Model Summary

The system consists of:

- Two fast variables: \( x(t), y(t) \)
- One slow internal variable: \( c(t) \)

A constraint-dependent boundary \( a(c) \) defines the region from which recovery is dynamically accessible.

As \( c \) increases, this boundary contracts.

---

## 🧪 Method Overview

- Initial conditions sampled over a grid in \( (x_0, y_0) \)
- Simulations performed via standard ODE integration
- A trajectory is classified as "recovered" if it returns to a neighborhood of the base attractor within a fixed time window
- The recoverable set is estimated as the fraction of initial conditions satisfying this condition

---

## 🔁 Reproducibility

All results are deterministic and reproducible from the provided code.

The implementation is intentionally minimal to allow independent verification and falsification.

---

## 🔗 Relation to ERC Framework

This work corresponds to:

- **Paper 1:** Minimal model (single trajectory perspective)  
- **Paper 2 (this document):** Ensemble-level behavior  
- **Paper 3:** Rate-dependent collapse (temporal forcing)

---

## ⚠️ Scope

This is a minimal dynamical model.

No claim is made that the system directly represents a specific physical or biological process.

Instead, it provides a conceptual and computational framework for studying loss of recoverability.

---

## 🤝 Contributions

Independent replication, critique, and extensions are welcome.
