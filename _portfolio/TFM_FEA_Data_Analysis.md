---
layout: single
title: "Displacement Field Extraction and Stress Reconstruction from Fluorescence Imaging"
excerpt: "Developed a data analysis pipeline to extract displacement fields from fluorescence microscopy and reconstruct stress distributions using particle tracking and finite element modeling."
categories: [Modeling-Simulation]
tags: [TFM, data analysis, particle tracking, MATLAB, Python, biomechanics, signal processing]

header:
  teaser: /assets/images/TFM_Data_Analysis.png
---

## Objective  
To develop a robust data analysis pipeline for converting **fluorescence microscopy data into quantitative mechanical information**, including displacement fields and stress distributions.

---

## Experimental Setup  
- Time-lapse fluorescence imaging was used to capture **motion of embedded fluorescent beads**.  
- Particle tracking algorithms (Trackpy) were applied to extract **displacement vectors across frames**.  
- Displacement data were filtered, interpolated, and mapped into a structured grid.  
- Processed data were used as input for **finite element-based stress reconstruction**.  

<img src="/assets/images/TFM_Displacement_Workflow.png" alt="TFM data processing workflow" width="700"/>  
*Figure 1: Data analysis pipeline from fluorescence imaging → particle tracking → displacement field reconstruction → stress estimation.*  

---

## Key Findings  
- Optimized particle tracking parameters significantly improved **displacement accuracy and robustness**.  
- Data filtering and interpolation reduced noise and enabled **stable stress reconstruction**.  
- The pipeline enabled consistent analysis across multiple datasets and experimental conditions.  

<img src="/assets/images/TFM_Displacement_Field.png" alt="Displacement field from bead tracking" width="700"/>  
*Figure 2: Displacement field extracted from fluorescent bead motion across the substrate.*  

---

## Outcome  
- Developed a reproducible pipeline for extracting **high-resolution displacement fields**.  
- Enabled transformation of imaging data into **quantitative stress and deformation maps**.  
- Integrated data analysis with computational modeling for end-to-end force quantification.  

---

## Engineering Contributions  
- Image processing and particle tracking (Python, MATLAB)  
- Data filtering and interpolation  
- Displacement field reconstruction  
- Integration with finite element modeling workflows  
