---
layout: splash
title: "Finite Element Mesh Sensitivity Analysis for Accurate Stress Reconstruction in TFM Substrates"
categories: [Modeling-Simulation]
tags: [FEA, Abaqus, mesh sensitivity, biomechanics, TFM, computational modeling, simulation optimization]

excerpt: "Performed mesh sensitivity analysis to optimize finite element discretization for accurate and computationally efficient stress reconstruction in micropatterned TFM substrates."

header:
  overlay_image: /assets/images/Mesh_Sensitivity_Analysis.png
  overlay_filter: 0.4
  caption: "Mesh sensitivity analysis for stress reconstruction in micropatterned substrates"
  teaser: /assets/images/TFM_FEA_Mesh_Generation.png
---

## Objective  

To determine the optimal finite element mesh configuration for accurate and computationally efficient reconstruction of stress fields in micropatterned PDMS substrates used in traction force microscopy (TFM–FEA workflow).

---

## Simulation Framework  

- Micropatterned substrate geometry (400 × 400 × 50 µm) was generated and imported into Abaqus.  
- Region of interest (ROI) defined as **200 × 200 × 50 µm** for localized stress analysis.  
- Displacement fields (from fluorescence imaging) were mapped as **nodal boundary conditions**.  
- Finite element simulations were performed to reconstruct **stress fields and strain energy density**.  

---

## Mesh Sensitivity Workflow  

<img src="/assets/images/TFM_FEA_Bead_Concentration.png" alt="Mesh sensitivity workflow" width="800"/>  

*Figure 1. Mesh sensitivity analysis workflow. Finite element simulations were performed across multiple mesh densities and thickness discretizations. Stress convergence and computational cost were evaluated to determine the optimal mesh configuration.*

<img src="/assets/images/TFM_FEA_Mesh_Generation.png" alt="Mesh generation and refinement" width="800"/>  

*Figure 2. Mesh generation and refinement strategy. Multiple mesh densities were generated to evaluate convergence behavior and numerical stability.*

---

## Parameter Study  

The following parameters were systematically varied:

- **Element density:** 0.01 → 0.64 µm⁻²  
- **Thickness discretization:** 5 → 20 elements  
- **Geometric nonlinearity (NLgeom):** Enabled vs disabled  

---

## Stress Convergence Analysis  

<img src="/assets/images/TFM_FEA_Mesh_Sensitivity_1.png" alt="Stress convergence plots" width="800"/>  

<img src="/assets/images/TFM_FEA_Mesh_Sensitivity_2.png" alt="Stress convergence plots" width="800"/>  

<img src="/assets/images/TFM_FEA_Noise_Analysis.png" alt="Noise analysis in stress fields" width="800"/>  

*Figure 3. Stress convergence analysis across different mesh densities. Coarse meshes produce noisy stress distributions, while refined meshes yield smooth and stable solutions.*

### Key Observations  

- Coarse meshes introduced **significant fluctuations in stress fields**  
- Mesh densities above ~0.09 µm⁻² produced **smooth and consistent results**  
- No meaningful improvement observed beyond **0.25 µm⁻²**  
- Over-refined meshes significantly increased **computational time**  

These trends highlight the importance of balancing **accuracy and computational efficiency** in biomechanical simulations.  

---

## Thickness Discretization Analysis  

### Key Findings  

- Coarse thickness meshes caused **stress variation across depth**  
- Convergence achieved at **~10 elements through thickness**  
- Further refinement (15–20 elements) showed **negligible improvement**  

---

## Effect of Geometric Nonlinearity  

- Maximum deformation ≈ **0.1 µm (~5% strain)**  
- Simulations with and without NLgeom showed **nearly identical results**  
- Enabling NLgeom significantly increased **computational cost**  

👉 Therefore, a **linear (small-strain) formulation** was selected for all simulations.  

---

## Key Findings  

- Optimal mesh density identified as **0.25 µm⁻²**  
- Minimum thickness discretization: **10 elements**  
- Stress reconstruction accuracy strongly depends on **mesh resolution**  
- Computational cost increases significantly beyond optimal mesh density  
- Linear formulation is sufficient for **small-strain biomechanical systems**  

---

## Outcome  

- Established a validated framework for **mesh-independent stress reconstruction**  
- Improved computational efficiency without compromising accuracy  
- Enabled reliable interpretation of **cell-generated stress fields**  
- Provided guidelines for **finite element modeling of soft biomaterials**  

---

## Engineering Contributions  

- Finite element modeling (Abaqus)  
- Mesh sensitivity and convergence analysis  
- Computational optimization (accuracy vs cost trade-off)  
- Stress field validation and reconstruction  
- Integration with experimental biomechanics (TFM data)  

---

## Impact  

This work ensures **robust and reliable stress quantification** in TFM–FEA workflows and provides a generalizable methodology for:

- Soft material simulation  
- Biomechanical modeling  
- Medical device design  
- Tissue engineering platforms  

By systematically optimizing mesh parameters, this study bridges **experimental imaging and computational mechanics**, enabling accurate interpretation of complex biological force systems.
