# 📄 Refractive Cosmology II (RC‑II)
**Airy‑like Modes of the Nonlinear Helmholtz Field**  
Status: *Manuscript in preparation (Overleaf project)*

---

## 📘 Overview

This directory contains all materials related to the RC‑II manuscript, which develops the **Airy‑like oscillatory modes** arising from the nonlinear Helmholtz field.  
These modes appear naturally in refractive geometry and provide:

- oscillatory corrections to rotation curves,  
- characteristic Airy‑like envelopes,  
- mode quantization linked to refractive saturation,  
- connections to soliton structure from RC‑I.

RC‑II extends the effective‑metric framework introduced in RC‑I and focuses on the **shape‑mode sector** of the nonlinear field.

---

## 📁 Directory Structure

```text
papers/RC-II/
│
├── manuscript/          # LaTeX source, figures, Overleaf export
│   ├── main.tex
│   ├── figures/
│   └── bibliography/
│
├── supplementary/       # Extra plots, mode analysis, extended derivations
│   ├── airy-profiles/
│   ├── mode-spectra/
│   └── asymptotics/
│
└── published/           # Final PDF (added after acceptance)

🔬 Reproducing Figures
Figures in RC‑II are generated using MATLAB/Python scripts located in:
src/matlab/fitting/
src/matlab/plotting/
src/matlab/utils/
Airy‑mode datasets and numerical outputs are stored in:
data/SPARC/processed/
data/SPARC/fits/
Each figure has a corresponding script and dataset.

📊 Airy‑Mode Workflow
Load galaxy data
src/matlab/loaders/load_sparc.m

Compute baseline soliton profile
(parameters 
𝑣
0
, 
𝑟
0
 from RC‑I)

Evaluate Airy‑like mode corrections
src/matlab/fitting/compute_airy_modes.m

Generate oscillatory envelopes and comparison plots
src/matlab/plotting/plot_airy_modes.m

Export mode spectra and residuals
papers/RC-II/supplementary/mode-spectra/

🧠 Theory Notes
Extended derivations for Airy‑like modes are located in:
docs/theory-notes/
docs/derivations/
Includes:

asymptotic expansion of the nonlinear Helmholtz field,

Airy‑mode envelope derivation,

mode quantization conditions,

connection to RC‑I effective metric.

📬 Citation
If you use RC‑II results, please cite:

P. Pintr, Refractive Cosmology II (2026)  
Repository: https://github.com/astropintr/Refractive-physics
