---
layout: splash
title: "Displacement Field Extraction and Stress Reconstruction from Fluorescence Imaging"
categories: [Modeling-Simulation]
tags: [TFM, data analysis, particle tracking, MATLAB, Python, biomechanics, signal processing]

excerpt: "Developed a computational pipeline to extract displacement fields from fluorescence microscopy and reconstruct stress distributions using particle tracking and finite element modeling."

header:
  overlay_image: /assets/images/TFM_FEA_Data_Analysis.png
  overlay_filter: 0.4
  caption: "Displacement field extraction and stress reconstruction workflow from fluorescence imaging data"
  teaser: /assets/images/TFM_FEA_Data_Analysis.png
---

## Objective  
To develop a robust data analysis pipeline for converting **fluorescence microscopy data into quantitative mechanical insights**, including displacement fields and stress distributions.

---

## Experimental Setup  
- Time-lapse confocal fluorescence imaging was used to capture **motion of embedded fluorescent beads**.  
- A template-matching approach was applied to define the **region of interest (ROI)** on micropatterned substrates.  
- Particle tracking algorithms (Trackpy) were used to extract **displacement vectors across time frames**.  
- Processed displacement data were used for **kinetic analysis and stress reconstruction**.  

---

## ROI Definition and Image Preprocessing  

<img src="/assets/images/TFM_FEA_Template_Matching.png" alt="ROI definition using template matching" width="800"/>  

*Figure 1. ROI selection using template matching. A template representing the micropattern geometry is matched to fluorescence images to define a consistent region of interest (ROI). The cropped ROI ensures accurate and repeatable displacement tracking across datasets.*  

---

## Kinematic Analysis of Displacement Fields  

<img src="/assets/images/TFM_FEA_Kinetic_Analysis.png" alt="Displacement and velocity analysis" width="800"/>  

*Figure 2. Displacement and velocity analysis of tracked bead motion. (A) Reference frame selection based on displacement magnitude. (B) Displacement evolution showing contraction and relaxation phases. (C) Velocity analysis highlighting peak contraction and relaxation rates.*  

---

## Data Processing and Stress Reconstruction Workflow  

<img src="/assets/images/TFM_FEA_Data_Analysis.png" alt="Data processing workflow" width="800"/>  

*Figure 3. Data processing workflow for displacement and stress analysis. Displacement fields from top and bottom planes are processed over time, subdivided into regions of interest (ROIs), and aggregated to extract representative displacement and stress metrics. Stress reconstruction is performed using finite element simulation outputs.*  

---

## Key Findings  
- Template matching enables **consistent ROI selection** across complex micropatterned geometries.  
- Optimized particle tracking improves **accuracy and robustness of displacement fields**.  
- Time-resolved analysis captures **contraction–relaxation dynamics** of the system.  
- ROI-based aggregation improves stability and reduces noise in **stress reconstruction**.  

---

## Outcome  
- Developed a reproducible pipeline for extracting **high-resolution displacement fields from imaging data**.  
- Enabled transformation of fluorescence imaging into **quantitative mechanical measurements**.  
- Integrated data analysis with computational modeling for **end-to-end biomechanics analysis**.  

---

## Engineering Contributions  
- Image processing and ROI definition  
- Particle tracking and displacement extraction  
- Time-series analysis and signal processing  
- Data aggregation and noise reduction  
- Integration with finite element modeling workflows  
