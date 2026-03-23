# Paper 3 – Rate-dependent Reachability Collapse

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.19189528.svg)](https://doi.org/10.5281/zenodo.19189528)

This document presents the temporal extension of the Endogenous Reachability Collapse (ERC) framework.

While previous work establishes that recoverability can be lost due to internal constraints, this paper investigates whether collapse depends not only on the magnitude of perturbation, but on the **rate at which it is applied**.

---

## 📌 Core Idea

The key question explored is:

> Does system collapse depend on how fast demand is applied relative to recovery timescales?

To test this, we introduce **time-dependent forcing** into the ERC framework.

---

## 🔍 Key Result

Numerical simulations suggest that:

> Collapse depends strongly on input rate, even when total input (AUC) is held constant.

This indicates that:

- Two perturbations with identical total load can produce different outcomes  
- Faster inputs may drive the system beyond its recoverable regime  
- Collapse emerges from a **timescale mismatch**, not only from magnitude  

---

## 📊 Contents

- `ERC-paper-3-rate-dependen`  
  Formal description of the rate-dependent model  

- `code/ercm_rate_model.ipynb`  
  Reproducible simulations with time-dependent forcing  

- `figures/`  
  Visualizations of:
  - recovery vs input rate  
  - collapse boundaries under different forcing profiles  
  - time evolution of system variables  

---

## ⚙️ Model Extension

This work extends the ERC framework by introducing:

- Time-dependent input (forcing)
- Control of rise time vs total input
- Explicit comparison of trajectories under matched AUC

The system remains minimal but incorporates a **temporal dimension**.

---

## 🧪 Method Overview

- Inputs are constructed as pulses with controlled rise time and fixed total area (AUC)
- Simulations performed via standard ODE integration
- Recovery is defined as return to a neighborhood of the base attractor within a fixed time window
- Collapse is evaluated across different input rates

---

## 🔁 Reproducibility

All simulations are deterministic and reproducible from the provided code.

The implementation is intentionally minimal to allow independent verification and falsification.

---

## 🔗 Relation to ERC Framework

This work corresponds to:

- **Paper 1:** Minimal model (existence of reachability collapse)  
- **Paper 2:** Ensemble behavior (recoverable fraction)  
- **Paper 3 (this document):** Rate-dependent collapse  

---

## ⚠️ Scope

This is a minimal dynamical model.

No claim is made that the system directly represents a specific physical or biological system.

Instead, it provides a conceptual framework for understanding how recovery may fail under time-dependent forcing.

---

## 🤝 Contributions

Independent replication, critique, and extensions are welcome.

This work extends the ERC framework introduced in Paper 1 and expanded in Paper 2.
