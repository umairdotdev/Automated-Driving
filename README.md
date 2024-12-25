
# Automated Driving

This repository showcases a collection of projects in the field of automated driving. It serves as a hub for various models, algorithms, and applications demonstrating core concepts and practical implementations in vehicle dynamics, control, and perception.

## Contents

1. **Lane Keeping Assist System**  
   **Description**: Implementation of a Lane Keeping Assist (LKA) system using Model Predictive Control (MPC).  
   **Key Features**:  
   - State-space modeling of lateral vehicle dynamics.  
   - Integration of road curvature preview and sensor dynamics for enhanced control.  
   - MPC-based steering control for lane tracking with smooth control inputs.  
   - Visualization of lateral deviation, yaw angle, and steering inputs.  
   **Folder**: [Lane-Keeping-Assist-System](./Lane-Keeping-Assist-System)  
   **Reference**: Based on [MathWorks' example](https://de.mathworks.com/help/mpc/ug/lane-keeping-assist-system-using-model-predictive-control.html).

2. **Adaptive Cruise Control (ACC) Using Model Predictive Control (MPC)**  
   **Description**: Implementation of an ACC system using Model Predictive Control (MPC).  
   **Key Features**:  
   - Dynamic lead vehicle simulation with sinusoidal acceleration profile.  
   - MPC-based control for maintaining safe distance and desired velocity.  
   - Nonlinear constraints for velocity and distance safety.  
   - Visualization of acceleration, velocity, and relative distance over time.  
   **Folder**: [Adaptive-Cruise-Contro-MPC](./Adaptive-Cruise-Control-MPC)  
   **Reference**: Inspired by [MathWorks' example](https://de.mathworks.com/help/mpc/ug/adaptive-cruise-control-using-model-predictive-controller.html).

---

## Usage

Clone the repository:  
```bash
git clone https://github.com/your-username/Automated-Driving.git
cd Automated-Driving
```

Explore individual project folders for instructions on running the implementations.

## Acknowledgments

This repository brings together concepts from vehicle dynamics, control theory, and automated driving.
