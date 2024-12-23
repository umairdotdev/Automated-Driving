# Lane Keeping Assist System using Model Predictive Control

## Description

This project implements a Lane Keeping Assist (LKA) system using Model Predictive Control (MPC). The LKA system helps vehicles maintain their position within a lane by optimizing steering control based on lateral deviation, relative yaw angle, and road curvature.

This implementation is based on the example provided by MathWorks: [Lane Keeping Assist System using Model Predictive Control](https://de.mathworks.com/help/mpc/ug/lane-keeping-assist-system-using-model-predictive-control.html).

This repository contains the Jupyter notebook for the implementation, simulations, and visualizations of the LKA system. The project demonstrates the effectiveness of MPC in maintaining lane position while ensuring smooth steering control.

## Features

- Implementation of lateral vehicle dynamics using a state-space model.
- Integration of road curvature previewer and sensor dynamics for enhanced lane tracking.
- MPC-based optimization for real-time steering control.
- Visualization of lateral deviation, relative yaw angle, and steering angle over time.

## Requirements

To run this project, you need the following dependencies installed:
- Python 3.8+
- Jupyter Notebook
- do-mpc
- CasADi
- NumPy
- Matplotlib

You can install the Python libraries using the following command:

```bash
pip install do-mpc casadi numpy matplotlib
```

## How to Use

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/lane-keeping-assist-mpc.git
   cd lane-keeping-assist-mpc
   ```
2. Open the Jupyter notebook:
   ```bash
   jupyter notebook Lane_Keepin_Assist_System.ipynb
   ```
3. Run the cells step by step to execute the simulation.

## Visualizations

The notebook includes visualizations of key variables over time, such as:
- Lateral deviation (meters)
- Relative yaw angle (radians)
- Steering angle (radians)

These plots provide insights into the system's performance.

## Acknowledgments

This project is inspired by the principles of vehicle dynamics and control. The curvature previewing and MPC setup are adapted to ensure real-time feasibility and accuracy.

The implementation is based on [MathWorks' Lane Keeping Assist System using Model Predictive Control](https://de.mathworks.com/help/mpc/ug/lane-keeping-assist-system-using-model-predictive-control.html).

---

**Note**: For detailed equations and explanations, refer to the markdown cells in the Jupyter notebook.
