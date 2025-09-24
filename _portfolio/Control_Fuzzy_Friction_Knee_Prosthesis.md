---
layout: single
title: "Impedance Control in Knee Prostheses using Fuzzy Friction Estimation"
categories: [Image/Data Analysis, Simulation & Control]
tags: [prosthesis, knee, impedance-control, fuzzy-logic, friction-estimation]
excerpt: "Integration of fuzzy logic-based friction estimation into an impedance control framework to enhance stability and adaptability of robotic knee prostheses."
teaser: /assets/images/Sarctrack_1.png 
---

## Objective  
The objective of this project was to **improve control strategies for robotic knee prostheses** by incorporating **fuzzy logic-based friction estimation** within an impedance control framework. This method compensates for nonlinear joint friction, thereby improving prosthesis stability and adaptability during gait.  

---

## Fuzzy Friction Estimation  

### Real vs. Estimated Torque  
<img src="/assets/images/Knee_Prosthesis_Friction_Estimation.png" alt="Comparison of real and estimated friction torque" width="700"/>  
*Figure 1: Comparison of measured (blue) and estimated (orange) friction torque, demonstrating the accuracy of fuzzy logic estimation.*  

### Fuzzy Membership Functions  
<img src="/assets/images/Knee_Prosthesis_Fuzzy_Estimator.png" alt="Membership functions used in fuzzy estimation" width="700"/>  
*Figure 2: Fuzzy membership functions used for friction estimation, mapping input motor velocity into fuzzy sets for robust nonlinear compensation.*  

### Fuzzy System Structure  
<img src="/assets/images/Knee_Prosthesis_Fuzzy_Friction_Estimation_Block.png" alt="Block diagram of fuzzy friction estimation system" width="600"/>  
*Figure 3: Fuzzy inference system used to estimate joint friction based on motor velocity and adaptive weights.*  

---

## Control Architecture with Fuzzy Friction Compensation  
<img src="/assets/images/Knee_Prosthesis_Workflow_Friction_Control_Plus_Fuzzy_Estimation_Block.png" alt="Impedance control with fuzzy friction estimation" width="900"/>  
*Figure 4: Integrated impedance control architecture with high-level state machine, mid-level impedance model, and low-level PI control enhanced by fuzzy friction estimation.*  

---

## Experimental Results  

### Swing Phase Trajectories  
<img src="/assets/images/Knee_Prosthesis_Result_1_Impedance_Control.png" alt="Knee joint angle and torque results with fuzzy control" width="700"/>  
*Figure 5: Knee joint angle (top) and torque (bottom) profiles under impedance control with fuzzy friction estimation.*  

### Motor Current Profiles  
<img src="/assets/images/Knee_Prosthesis_Result_2_Impedance_Control.png" alt="Motor current under impedance control with fuzzy estimation" width="700"/>  
*Figure 6: Motor current signals showing stable and consistent control effort with fuzzy friction compensation.*  

#  ### Friction Compensation in Motion  
#<img src="/assets/images/Knee_Prosthesis_Result_Friction.png" alt="Friction compensation result" width="600"/>  
#*Figure 7: Improved torque tracking with fuzzy friction estimation during cyclic motion.*  

#<img src="/assets/images/Knee_Prosthesis_Result_Friction_kinetics.png" alt="Knee angle and estimated friction profiles" width="600"/>  
#*Figure 8: Knee angle trajectory (top) and estimated friction torque (bottom), showing effective compensation during swing.*  

---

## Outcomes  
- Developed and validated a **fuzzy logic-based friction estimator** integrated into impedance control.  
- Achieved improved **tracking accuracy** and **stability** during swing phase.  
- Enhanced prosthesis adaptability to nonlinear joint dynamics and variable gait conditions.  
- Provided a robust control framework for future **intelligent prosthetic knee designs**.  
