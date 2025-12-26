# Scalar Field Dynamics in Cosmology

This repository contains numerical and theoretical analysis of a cosmological scalar field evolving in an expanding FLRW universe.  
The work is based on my **MSc Physics dissertation** and focuses on the dynamics of scalar fields with **steep exponential potentials**, motivated by dark energy and early dark energy scenarios.

---

## Overview

The project studies the evolution of a minimally coupled scalar field governed by the Friedmann and Klein–Gordon equations, including contributions from matter and radiation. The main goals are:

- To understand the dynamical behavior of scalar fields in cosmology  
- To study scaling and tracking solutions for steep exponential potentials  
- To analyze the evolution of the equation of state and density parameters  
- To explore implications for late-time acceleration and early dark energy  

---

## Repository Contents

- **`Dynamics of Scalar Field.ipynb`**  
  Jupyter notebook containing:
  - Numerical solution of Friedmann + Klein–Gordon equations  
  - Evolution of scalar field, Hubble parameter, and energy densities  
  - Equation of state analysis  
  - Comparison with ΛCDM behavior  

- **`MSc Project Thesis.pdf`**  
  Full MSc dissertation with:
  - Theoretical background (FLRW cosmology, scalar fields)  
  - Analytical derivations  
  - Numerical results and interpretation  

---

## Theoretical Framework

The action considered is:

\[
\mathcal{S} = \int d^4x \sqrt{-g}
\left[
\frac{M_{\text{Pl}}^2}{2} R
- \frac{1}{2} (\partial_\mu \phi)(\partial^\mu \phi)
- V(\phi)
\right]
\]

with a steep exponential potential of the form:

\[
V(\phi) = V_0 \exp\left(-\lambda \frac{\phi^n}{M_{\text{Pl}}^n}\right)
\]

The coupled Friedmann and Klein–Gordon equations are solved numerically.

---

## Numerical Method

- Time evolution is performed by numerically integrating coupled ODEs  
- Matter, radiation, and scalar field components are included  
- Initial conditions are chosen to study kinetic- and potential-dominated regimes  
- Results are tested for qualitative robustness under parameter variation  

---

## Requirements

To run the notebook, install the following Python packages:

```bash
pip install numpy scipy matplotlib jupyter
