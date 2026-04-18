---
layout: splash
title: "Finite Element Mesh Sensitivity Analysis for Accurate Stress Reconstruction in TFM Substrates"
categories: [Modeling-Simulation]
tags: [FEA, Abaqus, mesh sensitivity, biomechanics, TFM, computational modeling, simulation optimization]

excerpt: "Performed a systematic mesh sensitivity analysis to optimize finite element discretization for accurate and computationally efficient stress reconstruction in micropatterned TFM substrates."

header:
  overlay_image: /assets/images/Mesh_Sensitivity_Analysis.png
  overlay_filter: 0.4
  caption: "Mesh sensitivity analysis for stress reconstruction in micropatterned substrates"
  teaser: /assets/images/TFM_FEA_Mesh_Generation.png
---

## Objective  

To determine the optimal finite element mesh configuration for accurate and computationally efficient reconstruction of stress fields in micropatterned PDMS substrates within a TFM–FEA workflow.

---

## Simulation Framework  

- Micropatterned substrate geometry (400 × 400 × 50 µm) was modeled and imported into **Abaqus**.  
- Region of interest (ROI) defined as **200 × 200 × 50 µm** for localized analysis.  
- Displacement fields from fluorescence imaging were applied as **nodal boundary conditions**.  
- Finite element simulations were used to reconstruct **stress fields and strain energy density**.  

---

## Mesh Sensitivity Workflow  

<img src="/assets/images/TFM_FEA_Bead_Concentration.png" alt="Bead analysis workflow" width="800"/>  

<p style="font-size:0.9em; text-align:center;">
<strong>Figure 1.</strong> Experimental and simulated analysis of fluorescent bead characteristics used for displacement tracking. Bead dispersion, size, and intensity distributions were evaluated to validate tracking parameters and ensure robust displacement field reconstruction.
</p>

<img src="/assets/images/TFM_FEA_Mesh_Generation.png" alt="Mesh generation and refinement" width="800"/>  

<p style="font-size:0.9em; text-align:center;">
<strong>Figure 2.</strong> Micropatterned substrate geometry and finite element mesh generation. Mesh refinement was performed with varying element densities and through-thickness discretization to evaluate convergence behavior.
</p>

---

## Parameter Study  

The following parameters were systematically varied:

- **Element density:** 0.01 → 0.64 µm⁻²  
- **Thickness discretization:** 5 → 20 elements  
- **Geometric nonlinearity (NLgeom):** Enabled vs disabled  

---

## Stress Convergence Analysis  

<img src="/assets/images/TFM_FEA_Mesh_Sensitivity_1.png" alt="Stress convergence plots" width="800"/>  

<p style="font-size:0.9em; text-align:center;">
<strong>Figure 3.</strong> Mesh sensitivity analysis of maximum principal stress under a circular load (500 Pa). Stress distributions and profiles were evaluated along multiple directions for different mesh densities to assess convergence and computational cost.
</p>

<img src="/assets/images/TFM_FEA_Mesh_Sensitivity_2.png" alt="Thickness and NLgeom analysis" width="800"/>  

<p style="font-size:0.9em; text-align:center;">
<strong>Figure 4.</strong> Effect of through-thickness discretization and geometric nonlinearity on stress reconstruction. Convergence behavior and stress accuracy were analyzed across different mesh configurations.
</p>

<img src="/assets/images/TFM_FEA_Noise_Analysis.png" alt="Noise analysis in stress fields" width="800"/>  

<p style="font-size:0.9em; text-align:center;">
<strong>Figure 5.</strong> Noise analysis under cell-free conditions. Displacement and strain energy fields were evaluated to quantify baseline noise and validate robustness of the TFM–FEA pipeline.
</p>

---

### Key Observations  

- Coarse meshes introduced **significant fluctuations in stress fields**  
- Mesh densities above ~0.09 µm⁻² produced **smooth and stable results**  
- No meaningful improvement observed beyond **0.25 µm⁻²**  
- Over-refined meshes significantly increased **computational cost**  

These results highlight the importance of balancing **accuracy and computational efficiency** in biomechanical simulations.  

---

## Thickness Discretization Analysis  

### Key Findings  

- Coarse thickness meshes caused **stress variation across depth**  
- Convergence achieved at **~10 elements through thickness**  
- Further refinement (15–20 elements) showed **negligible improvement**  

---

## Effect of Geometric Nonlinearity  

- Maximum deformation ≈ **0.1 µm (~5% strain)**  
- Simulations with and without NLgeom showed **negligible differences**  
- Enabling NLgeom significantly increased **computational cost**  

👉 A **linear (small-strain) formulation** was therefore adopted.  

---

## Key Findings  

- Optimal mesh density: **0.25 µm⁻²**  
- Minimum thickness discretization: **10 elements**  
- Stress reconstruction strongly depends on **mesh resolution**  
- Computational cost increases beyond optimal refinement  
- Linear formulation is sufficient for **small-strain conditions**  

---

## Outcome  

- Established a framework for **mesh-independent stress reconstruction**  
- Improved computational efficiency without sacrificing accuracy  
- Enabled reliable quantification of **cell-generated forces**  
- Provided guidelines for **FEA modeling of soft biomaterials**  

---

## Engineering Contributions  

- Finite element modeling (Abaqus)  
- Mesh sensitivity and convergence analysis  
- Computational optimization (accuracy vs cost trade-off)  
- Stress field validation and reconstruction  
- Integration with experimental biomechanics (TFM data)  

---

## Impact  

This work enables **robust and reliable stress quantification** in TFM–FEA workflows and provides a generalizable methodology for:

- Soft material simulation  
- Biomechanical modeling  
- Medical device design  
- Tissue engineering platforms  

By optimizing mesh parameters, this study bridges **experimental imaging and computational mechanics**, enabling accurate interpretation of complex biological force systems.
