---
title: "TFM–FEA Integrated Workflow for Quantifying Cellular Forces"
excerpt: "Developed a full experimental–computational pipeline combining dual-plane imaging, particle tracking, and finite element analysis to quantify stress distribution on micropatterned substrates."
categories: [image-data-analysis]
tags: [TFM, FEA, Fluorescence Microscopy, MATLAB, Python, Abaqus]
layout: single
header:
teaser: /assets/images/TFM_FEA_Graphical_Abstract.png
---

## Objective  
Develop an end-to-end system to quantify cellular forces on non-planar micropatterned substrates by integrating traction force microscopy (TFM) with finite element analysis (FEA).


Methods Summary
- Dual-plane fluorescence imaging (top and bottom surfaces) was used to capture bead displacement.
- Particle tracking algorithms were applied to compute displacement fields.
- Displacement data were interpolated into a unified plane.
- Abaqus-based FEA was used to reconstruct stress and strain energy density fields.

<img src="/assets/images/TFM_FEA_Imaging_Workflow.png" width="700"/>

** Figure 1** . Integrated pipeline: imaging → particle tracking → displacement interpolation → finite element modeling → stress reconstruction.

## Outcome
- Developed a robust TFM–FEA pipeline for non-planar substrates
- Enabled quantitative analysis of cellular forces in engineered environments
- Integrated experimental imaging with computational modeling

⸻

## Impact

This system enables quantitative biomechanics analysis in complex geometries and provides a scalable framework for biomaterials design, organ-on-chip systems, and medical device testing.

⸻

## Engineering Contributions
- Experimental system design
- Image-based displacement tracking
- Finite element modeling (Abaqus)
- End-to-end system integration
