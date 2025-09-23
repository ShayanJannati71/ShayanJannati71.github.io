---
layout: single
title: "EMG Signal Processing for Locomotion Mode Classification and Knee Angle Estimation"
excerpt: "Developed machine learning and neural network models to classify locomotion modes and estimate knee joint kinematics from EMG signals, enabling adaptive control in prosthetic devices."
---

## Objectives  
This project leveraged surface electromyography (sEMG) signals for two primary goals:  
1. Classifying different locomotion modes using machine learning techniques, specifically Support Vector Machines (SVM).  
2. Estimating knee joint kinematics using neural network–based modeling to provide a reliable, non-invasive method for prosthetic control, rehabilitation, and human–machine interaction.  

## Methods  
- **Signal Acquisition & Processing:** sEMG signals were collected and pre-processed with filtering and normalization.  
- **Segmentation & Feature Extraction:** Time-series EMG data were segmented, and relevant features were extracted for analysis.  
- **Model Development:**  
  - **Locomotion Classification:** SVM was applied to classify locomotion modes.  
  - **Kinematics Estimation:** A Time-Delay Artificial Neural Network (TDANN) was designed to model nonlinear relationships between sEMG inputs and knee joint angles.  
- **Evaluation:** Performance was assessed using the coefficient of determination ($R^2$), evaluating the effects of varying delays and neuron counts on model accuracy.  

## Outcomes  
- SVM-based classification successfully differentiated between locomotion modes.  
- Increasing the number of delays decreased predictive accuracy, emphasizing the importance of optimized temporal windowing.  
- The TDANN achieved optimal performance with ~60 neurons, yielding $R^2 \approx 0.85$ for knee angle prediction.  
- Predicted knee angle trajectories closely matched target angles after filtering, demonstrating the robustness of the approach.  

## Figures  

**Workflow and Results**  
<img src="/assets/images/EMG_3.png" alt="Workflow of knee joint kinematics estimation using surface EMG and TDANN" width="600"/>  
*Figure 1: Workflow for knee joint kinematics estimation from sEMG using TDANN and evaluation of model performance.*

**Locomotion Mode Classification Results**  
<img src="/assets/images/EMG_1.png" alt="Locomotion Mode Classification using SVM" width="600"/>  
*Figure 2: SVM-based classification results for different locomotion modes.*

**Feature Extraction and Delay Analysis**  
<img src="/assets/images/EMG_2.png" alt="Effect of Number of Delays on Model Performance" width="600"/>  
*Figure 3: Effect of temporal delay settings on TDANN performance in knee angle prediction.*

**Knee Angle Estimation Results**  
<img src="/assets/images/EMG_3.png" alt="Filtered Knee Angle Estimation using TDANN" width="600"/>  
*Figure 4: Predicted vs. target knee joint angles after filtering, demonstrating accurate estimation using TDANN.*
