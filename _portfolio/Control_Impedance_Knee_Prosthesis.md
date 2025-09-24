---
layout: single
title: "Impedance Control for Knee Prosthesis in Swing Phase"
categories: [Modeling-Simulation,image-data-analysis]
tags: [prosthesis, knee, impedance-control, PI-controller, swing-phase]
excerpt: "Development of a multi-level impedance control strategy for robotic knee prostheses to improve performance during the swing phase of gait."
header:
  teaser: /assets/images/Knee_Prosthesis_Workflow_Impedance_Control.png
---

## Objective  
The goal of this project was to improve **control strategies for robotic knee prostheses** by implementing a **multi-level impedance control architecture** during the swing phase of gait. This approach enhances knee trajectory tracking, adaptability, and smoothness of motion.  

---

## Multi-Level Control Strategy  
The control framework integrates three hierarchical levels:  

1. **High-Level Control** – State machine defining swing phases (early vs. late).  
2. **Mid-Level Control** – Impedance model generating reference torque.  
3. **Low-Level Control** – PI controller ensuring torque tracking through motor actuation.  

<img src="/assets/images/Knee_Prosthesis_Workflow_Impedance_Control.png" alt="Workflow of impedance control for robotic knee prosthesis" width="800"/>  
*Figure 1: Multi-level control structure: state machine (high-level), impedance model (mid-level), and PI motor control (low-level).*  

---

## Experimental Results  

### Joint Angle and Torque Profiles  
<img src="/assets/images/Knee_Prosthesis_Result_1_Impedance_Control.png" alt="Knee angle and torque trajectories" width="700"/>  
*Figure 2: Measured knee joint angle (top) and corresponding torque (bottom) during swing phase, showing periodic and consistent tracking performance.*  

---

### Current and Motor Control  
<img src="/assets/images/Knee_Prosthesis_Result_2_Impedance_Control.png" alt="Motor current signals during impedance control" width="700"/>  
*Figure 3: Motor current profiles illustrating control effort and stability during swing trajectory tracking.*  

---

## Online Control and Sensor Validation  
<img src="/assets/images/Knee_Prosthesis_Workflow_Online_Control.png" alt="Validation of online control strategies using multiple sensors" width="800"/>  
*Figure 4: Online testing of swing phase control. Left: high-level swing test with trajectory tracking. Middle: incremental encoder validation. Right: absolute encoder validation with filtered knee angle signals.*  

---

## Outcomes  
- Implemented a **hierarchical impedance control strategy** for swing phase.  
- Achieved **stable trajectory tracking** for knee angle and torque.  
- Demonstrated effective **sensor integration** using both incremental and absolute encoders.  
- Enabled a robust framework for testing advanced **prosthetic gait control algorithms**.  
