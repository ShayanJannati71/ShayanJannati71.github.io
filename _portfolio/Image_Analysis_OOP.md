---
title: "Automated Image Processing for Cardiac Cell Orientation Measurement"
excerpt: "Developed an automated pipeline for quantifying cardiac cell alignment and orientation on micropatterned substrates."
categories: [image-data-analysis]
tags: [Image Analysis, Orientation, Cardiac Cells, Micropatterning, MATLAB, CellProfiler]
layout: single
header:
  teaser: /assets/images/Logo_OOP.png
---

## Objective  
Develop an automated pipeline to measure the orientation of cardiac cells cultured on micropatterned substrates.  

---

## Outcome
- Provides objective and reproducible **orientation metrics** of cardiac cells.  
- Enables **high-throughput screening** of alignment across substrate conditions.  
- Supports investigation of how microenvironmental cues guide **cellular organization**.  

---

## Workflow  

<img src="/assets/images/Image_Analysis_OOP_1.png" alt="Cardiac cell orientation workflow" width="500"/>  

**Figure 1.** Workflow for orientation measurement. Images are processed through filtering, morphological operations, and object detection in MATLAB, followed by orientation analysis in CellProfiler to generate orientational maps and order parameters.  

---

## Results  

<img src="/assets/images/Image_Analysis_OOP_2.png" alt="Orientation measurement results" width="900"/>  

**Figure 2.** Representative results of orientation analysis:  
- **(i)** Original α-actinin2 (green) images with nuclei (blue).  
- **(ii)** Processed skeletonized Z-lines.  
- **(iii)** Orientational maps showing alignment with micropattern direction.  
- **(iv)** Polar plots and order parameter analysis quantifying alignment across regions.  

---

## Impact  
This automated workflow provides a robust method to **quantify cardiac cell orientation** at scale.  
It can be applied to optimize **micropatterning strategies**, evaluate **substrate designs**, and study **mechanobiological responses** in cardiac tissue engineering.  
