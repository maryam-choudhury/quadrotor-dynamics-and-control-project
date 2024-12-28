# 🚁 Quadrotor Control and Simulation Project
#### quadrotor-dynamics-and-control
---

## 📖 **Project Overview**

This project focuses on developing a dynamic quadrotor control system. It was completed as a part of a Build Fellowship, and this repository is a fork of our mentor, Roy Vorster's, [tutorial repo](https://github.com/RoyVorster/oa-project). Each week-file builds on the previous week’s work. The ultimate goal of the project and fellowship experience was to build a robust simulation environment and control system for a quadrotor capable of stable flight and trajectory tracking under realistic conditions.


---

## **⚙️ Program Components**

### **1. Dynamics**
- **Purpose**: Model the physical behavior of the quadrotor under applied forces and torques.
- **Key Features**:
  - Computes linear and angular accelerations.
  - Accurate quaternion-based orientation updates.
  - Full 3D dynamics that consider inertia, gravity, and rotor thrust.

### **2. Controller**
- **Purpose**: Maintain stability and follow desired trajectories.
- **Key Features**:
  - PD control for altitude, position, and orientation.
  - Error correction using quaternion-based orientation differences.
  - Tuned gains for smooth and responsive control.

### **3. Trajectory**
- **Purpose**: Define target positions and orientations for the quadrotor.
- **Key Features**:
  - Basic trajectories with step-wise motion (`JumpTrajectory`).
  - Smooth trajectories with sinusoidal and circular transitions (`SmoothTrajectory`).

### **4. Simulation**
- **Purpose**: Simulate quadrotor flight and validate control strategies.
- **Key Features**:
  - Modular framework that integrates the previous components: dynamics, controller, and trajectory.
  - Real-time animation.

---


## 💻 **Technical Skills Practiced**

- **Mathematical Modeling**:
  - Quaternion algebra for orientation representation.
  - Dynamics equations for calculating angular acceleration and linear acceleration.
  - Mixing matrix for translating thrust and torque into rotor rates.

- **Visualization and Debugging**:
  - Used `k3d` to visualize the quadrotor’s flight in 3D.
  - Explored the effects of tuning control gains on system behavior.

