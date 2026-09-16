# 📄 Refractive Cosmology I (RC‑I)
**Effective Metric from the Nonlinear Helmholtz Field**  
Status: *Under review at Classical and Quantum Gravity (CQG)*

---

## 📘 Overview

This directory contains all materials related to the RC‑I manuscript:

- full LaTeX source (Overleaf export),
- figures used in the paper,
- supplementary plots,
- data and scripts required for reproduction.

The goal of RC‑I is to demonstrate that the nonlinear Helmholtz field generates an **effective refractive metric**, producing:

- dark‑matter–like solitons,  
- flat rotation curves,  
- Airy‑like oscillatory modes,  
- cosmological scaling relations.

---

## 📁 Directory Structure

```text
papers/RC-I/
│
├── manuscript/          # LaTeX source, figures, Overleaf export
│   ├── main.tex
│   ├── figures/
│   └── bibliography/
│
├── supplementary/       # Extra plots, tables, extended analysis
│   ├── collapse-plots/
│   ├── residuals/
│   └── parameter-studies/
│
└── published/           # Final PDF (added after acceptance)

🔬 Reproducing Figures
All figures in the RC‑I manuscript can be reproduced using scripts in:
src/matlab/fitting/
src/matlab/plotting/
src/matlab/loaders/

SPARC data used for rotation‑curve fits:
data/SPARC/
Each figure has a corresponding script and dataset.

📊 SPARC Fit Workflow
Load galaxy data
src/matlab/loaders/load_sparc.m

Perform two‑stage fit

Stage 1: determine 
𝑣
0
, 
𝑟
0

Stage 2: fit shape parameter 
𝛼

Generate collapse plots
src/matlab/plotting/plot_collapse.m

Export residuals and comparison tables
data/SPARC/fits/

📬 Citation
If you use RC‑I results, please cite:

P. Pintr, Refractive Cosmology I (2026)  
Repository: https://github.com/astropintr/Refractive-physics
