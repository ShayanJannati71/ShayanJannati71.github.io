---
layout: single
title: "TFM–FEA Integrated Workflow for Quantifying Cellular Forces"
excerpt: "Developed an experimental–computational pipeline combining dual-plane fluorescence imaging, particle tracking, and finite element analysis (FEA) to reconstruct stress fields on micropatterned substrates."
categories: [Modeling-Simulation]
tags: [TFM, FEA, fluorescence microscopy, MATLAB, Python, Abaqus, biomechanics]

header:
  teaser: /assets/images/TFM_FEA_Graphical_Abstract.png
---

## Objective  
To develop an integrated workflow for quantifying **cell-generated forces on non-planar micropatterned substrates** by combining **traction force microscopy (TFM)** with **finite element analysis (FEA)**.

---

## Experimental Setup  
- Dual-plane fluorescence imaging was used to capture bead displacement at the **top and bottom surfaces** of the micropatterned substrate.  
- Particle tracking algorithms were applied to determine **displacement fields** from fluorescent bead motion.  
- Displacement data from both planes were interpolated into a unified plane and mapped into **Abaqus** as boundary conditions.  
- Finite element analysis was used to reconstruct **stress fields** and **strain energy density**.  

<img src="/assets/images/TFM_FEA_Imaging_Workflow.png" alt="Integrated TFM-FEA workflow" width="700"/>  
*Figure 1: Integrated workflow combining dual-plane imaging, particle tracking, displacement interpolation, and finite element modeling for stress reconstruction.*  

---

## Key Findings  
- Developed a robust **TFM–FEA pipeline** for force quantification on non-planar substrates.  
- Dual-plane imaging improved displacement reconstruction across **micropatterned geometries**.  
- The workflow enabled spatial mapping of **stress distribution** and **strain energy density** in engineered substrates.  

<img src="/assets/images/TFM_FEA_Graphical_Abstract.png" alt="TFM-FEA graphical abstract" width="700"/>  
*Figure 2: Overview of the integrated experimental–computational framework for quantifying cellular mechanics on micropatterned substrates.*  

---

## Outcome  
- Established a complete **experimental–computational biomechanics workflow**.  
- Enabled quantitative analysis of cellular force transmission in engineered microenvironments.  
- Integrated imaging, data processing, and simulation into a single reproducible framework.  
- Published in *Biofabrication* (2026). **DOI:** [10.1088/1758-5090/ae573e](https://doi.org/10.1088/1758-5090/ae573e)

---

## Engineering Contributions  
- Experimental system design  
- Image-based displacement tracking  
- Data interpolation and preprocessing  
- Finite element modeling in Abaqus  
- End-to-end workflow integration
