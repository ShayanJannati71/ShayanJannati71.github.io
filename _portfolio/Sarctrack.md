---
layout: single
title: "Automated Sarcomere Tracking with SarcTrack"
categories: [image-analysis, biomechanics, cardiac]
tags: [Sarcomere, hiPSC-CM, image-processing, wavelet, Python]
excerpt: "Automated analysis of sarcomere dynamics in hiPSC-CMs using double-wavelet fitting and signal tracking."
---

## Objective  
To measure sarcomere dynamics (length, contraction, and relaxation velocities) in hiPSC-CMs using the **SarcTrack** algorithm for automated image-based analysis.  

## Methods  
- **Imaging:** GFP-tagged Z-lines imaged in hiPSC-CMs.  
- **Double-wavelet fitting:** Tracks distances between adjacent Z-lines across frames.  
- **Data processing:** Extracts frame-by-frame sarcomere lengths, then averages across cells.  
- **Outputs:**  
  - Maximum and minimum sarcomere length  
  - Peak contraction velocity  
  - Peak relaxation velocity  

**Workflow Illustration**  
<img src="/assets/images/Sarctrack_1.png" alt="SarcTrack workflow for automated sarcomere tracking" width="800"/>  
*Figure 1: SarcTrack workflow. GFP-tagged Z-lines are tracked across frames using double-wavelet fitting, yielding sarcomere length traces for contraction-relaxation cycles.*

## Outcomes  
- Enabled **high-throughput, automated analysis** of sarcomere contraction.  
- Provided quantitative insights into **cellular contractility and disease phenotypes** in hiPSC-CMs.  
- Forms a foundation for **AI-augmented sarcomere analysis pipelines** in future work.  

