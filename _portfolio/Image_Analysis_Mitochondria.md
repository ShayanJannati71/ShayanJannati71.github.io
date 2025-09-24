---
title: "Automated Mitochondrial Characterization in Cardiac Cells"
excerpt: "Developed an automated pipeline for mitochondrial segmentation and quantification in hiPSC-CMs using multi-channel fluorescence imaging."
categories: [image-data-analysis]
tags: [Image Analysis, Fluorescence Microscopy, Mitochondria, Cardiac Cells, MATLAB, CellProfiler]
layout: single
header:
  teaser: /assets/images/Image_Analysis_Mito_1.png
---

## Objective  
Develop an automated pipeline to characterize mitochondrial structure and distribution in cardiac cells using multi-channel fluorescence imaging.  

## Outcome *(in progress)*  
- Enables accurate segmentation and quantification of mitochondria.  
- Provides objective metrics of mitochondrial **intensity, size, and shape**.  
- Supports **high-throughput analysis** of cardiac cell organization and function.  

---

## Workflow  

<img src="/assets/images/Image_Analysis_Mito_1.png" alt="Automated Image Analysis Pipeline" width="400"/>  

**Figure 1.** Workflow for automated mitochondrial analysis. Images undergo Coherence Enhancing Anisotropic Diffusion filtering, Top-Hat filtering, thresholding, and cleaning in MATLAB, followed by object detection and quantitative measurement in CellProfiler.  

---

## Multi-Channel Imaging  

<img src="/assets/images/Image_Analysis_Mito_2.png" alt="Multi-channel fluorescence imaging" width="800"/>  

**Figure 2.** Multi-channel fluorescence imaging of hiPSC-derived cardiomyocytes.  
- Nuclei stained with Hoechst (blue)  
- Sarcomeres labeled with α-actinin2 (green)  
- Mitochondria labeled with Mitotracker (red)  
- Merged image shows integrated cellular architecture.  

---

## Results  

<img src="/assets/images/Image_Analysis_Mito_3.png" alt="Quantitative analysis of mitochondrial structure" width="800"/>  

**Figure 3.** Quantitative analysis of cardiac cells cultured on substrates of varying stiffness and patterning.  
- **Left:** Nucleus aspect ratio increases with micropatterning and stiffness.  
- **Right:** Normalized mitochondrial area differs significantly across conditions, highlighting the effect of microenvironment on organelle distribution.  

---

## Impact  
This automated analysis pipeline provides a scalable tool for **quantitative characterization of mitochondria** in cardiac cells.  
It can be extended to evaluate **disease models, drug responses, and tissue engineering approaches**, accelerating discovery in mechanobiology and cardiac research.  

