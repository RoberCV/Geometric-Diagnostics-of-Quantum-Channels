# Quantum Channel Geometry: Diagnostics, Calibration Protocols and Robustness
## Code for the Paper: Geometric Invariants of Quantum Channels: A Framework for Robustness and Noise Diagnostics
This repository contains the complete, Colab-ready Python implementation of all numerical experiments, figures, and diagnostic tools introduced in the paper. The notebooks provide a unified computational framework for studying the geometry of quantum channels under the Bures metric, including dynamical trajectories, geometric efficiency, curvature-weighted robustness, and parameter-sweep diagnostics.

All code is clean, fully commented in English, disk-free (no file writes), and generates all figures inline with outputs stored directly in Python variables or DataFrames.

### Repository Structure
#### 1. Parameter Sweep Diagnostics

Notebook: GI_5_2_1_Parameter_sweep_diagnostics.ipynb
Implements Section 5.2.1 of the paper.

Includes:

Fidelity, Bures distance, GDI, GAC across noise parameters

Diagnostic curves for dephasing, depolarizing, and amplitude-damping channels

Haar-random state sampling

Geometry of induced quantum trajectories

#### 2. Local Fragility and Sensitivity

Notebook: GI_5_2_2_Local_fragility_and_sensitivity.ipynb
Implements Section 5.2.2.

Includes:

Bures speed and acceleration along trajectories

Sensitivity to noise-parameter perturbations

Numerical computation of local fragility

Mean-over-states diagnostics

#### 3. Geometric Calibration Protocols

Notebook: GI_5_2_3_Geometric_calibration_protocols.ipynb
Implements Section 5.2.3.

Protocols implemented:

P1: Fixed depth

P2: Equal final fidelity

P3: Equal Bures length

Each protocol computes:

Cross-channel comparisons

GDI/GAC benchmarking

Robust parameter selection using bisection or grid search

Inline generation of all figures

#### 4. Curvature-Weighted Global Robustness

Notebook: GI_5_2_4_Curvature_weighted_global_robustness.ipynb
Implements Section 5.2.5.

Includes:

Curvature-weighted instability (CWI)

Global curvature robustness score (CRS)

Normalized cross-channel comparison

Figures:

CWI vs parameter

CRS vs parameter

1×3 panel per channel

#### 5. Case Study: Fiber-Induced Dephasing

Notebook: GI_Case_study_fiber_induced_dephasing.ipynb
Implements the case study in Section 5.3.

Includes:

Physical model of fiber-induced dephasing:
p_phi(L) = 1 - exp(-L / L_phi)

Distance-dependent degradation

Quantum Fragility Factor (QFF)

CWI/CRS along optical fiber links

Local speed/acceleration analysis

Full figure suite, inline

#### Key Concepts Implemented

Quantum trajectories under iterated Kraus channels

Bures geometry: fidelity, distance, speed, acceleration

Geometric trajectory efficiency:

GDI = LB / DB

GAC = mean angular alignment

Curvature-weighted instability (CWI)

Curvature robustness score (CRS)

Quantum fragility factor (QFF)

Haar-random state sampling

Cross-channel geometric benchmarking

### Running the Notebooks

All notebooks are self-contained and require only:

numpy
scipy
matplotlib
pandas

They run natively in:

Google Colab

Jupyter Notebook / JupyterLab

VSCode Python notebooks

### Citation

If you use this repository for academic work, please cite the accompanying paper: Not Available (review time)

### Contact

For questions, comments, or collaborations, please open an issue or contact:

Roberto Casado — rober@usal.es
