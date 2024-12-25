# Adaptive Cruise Control (ACC) Using Model Predictive Control (MPC)

This project implements an **Adaptive Cruise Control (ACC)** system using **Model Predictive Control (MPC)** with the `do-mpc` library. The goal is to ensure safe vehicle following by maintaining a safe distance from the lead vehicle while adhering to a set velocity whenever possible.

---

## Features

1. **Dynamic Lead Vehicle Simulation**:
   - The lead vehicle's motion is modeled with a sinusoidal acceleration profile, ensuring a realistic and varying behavior.

2. **MPC-based Control**:
   - Formulates the ACC problem as an optimization problem.
   - Controls acceleration (`a_ego`) as the primary input to achieve desired outcomes.

3. **Safety and Performance Objectives**:
   - Maintains a safe distance (`D_safe`) between the ego and lead vehicles.
   - Ensures the ego vehicle follows a set velocity (`v_set`) when safe.

4. **Nonlinear Constraints**:
   - Velocity constraint: The ego vehicle's velocity is bounded above to ensure safety.

5. **Simulation and Visualization**:
   - Plots the ego and lead vehicles' acceleration, velocity, and relative distance over time.
   - Demonstrates the controller's effectiveness in maintaining safe distances.

---

## How It Works

1. **State Variables**:
   - Ego vehicle: Position (`x_ego`), velocity (`v_ego`).
   - Lead vehicle: Position (`x_lead`), velocity (`v_lead`).

2. **Control Input**:
   - Acceleration of the ego vehicle (`a_ego`).

3. **Constraints**:
   - The actual distance (`D_relative`) must always be greater than or equal to the safe distance (`D_safe`).
   - Upper bound on ego vehicle's velocity (`v_ego` ≤ 30 m/s).

4. **Optimization Objective**:
   - Minimize the deviation between `D_relative` and `D_safe`.
   - Minimize control effort (`a_ego`).

5. **Results**:
   - The ego vehicle adjusts its acceleration to maintain safety and follow the lead vehicle efficiently.
   - Demonstrated using time-series plots for acceleration, velocity, and relative distance.

---

## Installation

### Requirements
- Python 3.7+
- `numpy`
- `matplotlib`
- `casadi`
- `do-mpc`

## How to Use

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/Adaptive-Cruise-Control-MPC.git
   cd Adaptive-Cruise-Control-MPC
   ```
2. Open the Jupyter notebook:
   ```bash
   jupyter notebook ACC.ipynb
   ```
3. Run the cells step by step to execute the simulation.

## Acknowledgments

This project is inspired by the principles of vehicle dynamics and control. The curvature previewing and MPC setup are adapted to ensure real-time feasibility and accuracy. This implementation was inspired by a MathWorks example [MathWorks' Adaptive Cruise Control System Using Model Predictive Control](https://de.mathworks.com/help/mpc/ug/adaptive-cruise-control-using-model-predictive-controller.html). The parameters used were adapted from their documentation, but the code and implementation are original

---

**Note**: For detailed equations and explanations, refer to the markdown cells in the Jupyter notebook.

