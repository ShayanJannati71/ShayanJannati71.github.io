---
layout: single
title: "EMG Signal Processing for Locomotion Classification and Knee Angle Estimation"
categories: [image-data-analysis]
tags: [EMG, locomotion, prosthetics, neural-networks, SVM, Python]
excerpt: "Developed machine learning and neural network models to classify locomotion modes and estimate knee joint kinematics from EMG signals, enabling adaptive prosthetic control and rehabilitation applications."

header:
 teaser: /assets/images/EMG_Data_Acquisition.png
---

## Objectives  
This project utilized surface electromyography (sEMG) signals with two primary goals:  
1. **Locomotion Classification** – Using Support Vector Machines (SVM) to identify walking modes.  
2. **Knee Joint Angle Estimation** – Applying a Time-Delay Artificial Neural Network (TDANN) to predict joint kinematics as a non-invasive solution for prosthetic control, rehabilitation, and human–machine interaction.  

---

## Methods  

### Signal Acquisition & Processing  
sEMG signals were collected from the **Rectus Femoris, Vastus Lateralis, Vastus Medialis, and Biceps Femoris** muscles. Signals were filtered, normalized, and synchronized with **IMU sensors** attached near the knee joint.  

<img src="/assets/images/EMG_Data_Acquisition.png" alt="sEMG and IMU data acquisition setup" width="600"/>  
*Figure 1: Experimental setup showing electrode placement, IMU sensor attachment, and data acquisition hardware.*  

<img src="/assets/images/EMG_Raw_Data.png" alt="Raw sEMG and IMU signals" width="600"/>  
*Figure 2: Example of raw sEMG signals (four muscles) with synchronized IMU data from the knee joint.*  

---

### Segmentation & Feature Extraction  
The time-series data were segmented into windows, and statistical and temporal features were extracted for classification and regression tasks.  

---

### Locomotion Classification (SVM)  
A Support Vector Machine (SVM) model was trained to classify locomotion modes based on extracted features.  

<img src="/assets/images/EMG_Workflow_Locomotion_Mode.png" alt="Workflow for locomotion classification using SVM" width="600"/>  
*Figure 3: Workflow for locomotion mode classification using sEMG features and SVM.*  

<img src="/assets/images/EMG_Confusion_Matrix.png" alt="Confusion matrix for SVM classification" width="600"/>  
*Figure 4: Confusion matrix illustrating classification performance across locomotion modes.*  

---

### Knee Joint Angle Estimation (TDANN)  
A Time-Delay Artificial Neural Network (TDANN) was implemented to capture nonlinear relationships between sEMG signals and knee joint angles. Different neuron counts and delay parameters were tested to optimize predictive accuracy.  

<img src="/assets/images/EMG_Knee_Angle_Estimation.png" alt="Workflow and results for knee joint angle estimation using TDANN" width="600"/>  
*Figure 5: Workflow of TDANN-based knee angle estimation, with predicted vs. actual trajectories.*  

---

## Evaluation  
Model performance was assessed using the **coefficient of determination (R²)**, with experiments exploring the effects of varying time delays and hidden neurons.  

---

## Outcomes  
- **Locomotion Classification:** SVM accurately differentiated between locomotion modes.  
- **Knee Angle Estimation:** TDANN achieved optimal performance with ~60 neurons, yielding **R² ≈ 0.85** for knee angle prediction.  
- **Temporal Analysis:** Increasing the number of time delays reduced accuracy, highlighting the need for optimal windowing.  
- **Robustness:** Predicted knee trajectories closely matched ground truth after filtering, confirming reliability for prosthetic and rehabilitation use cases.  
 




