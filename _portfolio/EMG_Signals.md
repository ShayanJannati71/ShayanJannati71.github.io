---
layour: single
title: "EMG Signals: Preprocessing & Feature Extraction"
date: 2025-09-23
categories: [signal‐processing, EMG, machine-learning]
tags: [EMG, filtering, Python, features]
excerpt: "Analysis of raw EMG signals, preprocessing and features extraction insights."
---


## Objectives  
This project leveraged surface electromyography (sEMG) signals for two primary goals:  
1. Classifying different locomotion modes using machine learning techniques, specifically Support Vector Machines (SVM).  
2. Estimating knee joint kinematics using neural network–based modeling, providing a reliable, non-invasive approach for prosthetic control, rehabilitation, and human–machine interaction.  

## Methods  
- **Signal Acquisition & Processing:** sEMG signals were collected from multiple muscles (Rectus Femoris, Vastus Lateralis, Vastus Medialis, and Biceps Femoris) and pre-processed using filtering and normalization.

**sEMG Signals Aquisition experimental setup for data aquisition**

<img src="/assets/images/EMG_5.png" alt="sEMG signals Experimental" width="600"/>  
*Figure 1: Example sEMG signals collected from major lower limb muscles during locomotion tasks.*

**sEMG Signals from Lower Limb Muscles**  
<img src="/assets/images/EMG_1.png" alt="sEMG signals from Rectus Femoris, Vastus Lateralis, Vastus Medialis, and Biceps Femoris" width="600"/>  
*Figure 1: pure sEMG signals and teh IMU data collected at the ame time.*

- **Segmentation & Feature Extraction:** Time-series EMG data were segmented, and relevant temporal and statistical features were extracted.

**Locomotion Mode Classification Using SVM**  
<img src="/assets/images/EMG_2.png" alt="Locomotion Mode Classification using SVM" width="600"/>  
*Figure 2: Confusion matrix showing SVM classification accuracy across multiple locomotion modes.*

**TDANN Workflow and Knee Angle Estimation Results**  
<img src="/assets/images/EMG_3.png" alt="Workflow of knee joint kinematics estimation using TDANN" width="600"/>  
*Figure 3: Workflow for knee joint kinematics estimation from sEMG using TDANN, along with predicted vs. actual knee angle trajectories.*
 
- **Model Development:**  
  - **Locomotion Classification:** SVM was used to classify locomotion modes.  
  - **Kinematics Estimation:** A Time-Delay Artificial Neural Network (TDANN) was designed to capture nonlinear relationships between sEMG inputs and knee joint angles.  
- **Evaluation:** Model performance was assessed using the coefficient of determination ($R^2$), examining the influence of varying time delays and neuron counts on predictive accuracy.  

## Outcomes  
- SVM-based classification accurately differentiated between locomotion modes.  
- Increasing the number of time delays reduced predictive accuracy, highlighting the importance of optimized temporal windowing.  
- The TDANN achieved optimal performance with ~60 neurons, yielding $R^2 \approx 0.85$ for knee angle prediction.  
- Predicted knee angle trajectories closely matched target angles after filtering, demonstrating the robustness of the approach.  




