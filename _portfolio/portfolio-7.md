---
title: "RDS 2025: Robotic Hand Control System"
excerpt: "Designed tendon-based kinematics and control software for a multi-DOF robotic hand with SEA-based compliant actuation and real-time CAN communication.<br/><img src='/images/hand.gif'>"
collection: portfolio
---

📍 **Institution**: Northwestern University — Robotics Design Studio  
🛠️ **Role**: Software Team (Kinematics & Control)  
📅 **Duration**: Jan 2025 – Jun 2025  

---

## Overview

RDS 2025 is a fully integrated robotic hand system composed of a 2-DOF wrist, 4-DOF dexterous finger, and 1-DOF power finger. The system employs **Series Elastic Actuators (SEA)** and **tendon-driven actuation**, managed through a multi-layered microcontroller architecture over **CAN bus**.

<br/><img src='/images/hand.gif'>

I contributed to the **software team**, specifically help with:
- **Joint-space and tendon-space kinematics**
- **Torque mapping and null-space control**
- **Low-/high-level PID control pipelines**

---

## System Contributions

### 🧠 Kinematics & Control Logic
- Developed tendon-to-joint velocity mapping via a Jacobian matrix.
- Supported null-space torque for tendon pretension and stability.
- Verified real-time performance with <100 ms control latency.

### 💡 SEA Force Modeling
- Calibrated force-deflection mappings for all linear and nonlinear SEAs.
- Integrated force curves into real-time force control feedback loops.

### ⚙️ Distributed Microcontroller Control
- Built state-machine and coordination logic for high-level controller (Teensy 4.1).
- Integrated joint-space PD control with SEA-based torque outputs to low-level MCUs.

### 📡 CAN Bus Communication
- Developed and debugged multi-node CAN protocols using [`rds25-comms`](https://github.com/NU-RDS/rds25-comms).
- Achieved reliable inter-device synchronization between wrist, dexterous finger, power finger, and palm controller.

### 🖥️ GUI & Debugging
- Supported Python-based Tkinter GUI with real-time plotting, system configuration, and diagnostic tools.
- Enabled position command streaming, error recovery, and calibration via interactive interface.

---

## Results & Impact

- ✅ Real-time SEA-based force control with ±0.1N accuracy.
- ✅ Full hand system tested with all DOFs under unified kinematic and communication framework.
- ✅ Modular software design enabled incremental hardware bring-up and multi-phase integration.

---
