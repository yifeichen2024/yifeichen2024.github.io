---
title: "Unitree G1 Humanoid Motion Control Deployment"
excerpt: "Developed and deployed high-/low-level motion control framework for Unitree G1 humanoid robot, enabling dual-arm Dex3 manipulation, whole-body motion policies, and real-time multi-policy ONNX deployment. <br/><img src='/images/g1_dance.gif'>  <br/><img src='/images/teleop.gif'>"
collection: portfolio
---

**Organization**: STARBOT INC — Santa Barbara, United States  
**Role**: Humanoid Motion Control Algorithm Engineer  
**Duration**: Jun 2025 – Aug 2025

---

## Overview

Designed and deployed a **comprehensive high- and low-level control system** for the **Unitree G1 humanoid robot**, integrating dual-arm manipulation with **Dex3 hands**, whole-body locomotion policies from  simulation (PBHC), and safety-checked real-time multi-policy switching.

---

## Highlights

- 🦾 **Dual-Arm + Dex3 Manipulation**:  
  Implemented coordinated arm-hand control with joint space & workspace trajectory recording/replay, triggered via gamepad or vision-based QR detection.
  
- ⚙️ **Whole-Body Motion Deployment**:  
  Executed locomotion and stance policies trained in simulation on the real robot, with safe state transitions and automatic fallback.

- 🔁 **Multi-Policy ONNX Pipeline**:  
  Built runtime switching between locomotion and stance controllers with hardware torque/velocity limit checks.

- 📐 **Advanced IK Integration**:  
  Combined **Pinocchio** and **CasADi** for smooth inverse kinematics solutions in coordinated arm control.

- 📷 **Vision-Based Triggers**:  
  Integrated **RealSense + QRDet** for spatially-aware and angle-gated teleoperation sequence triggering.

---
<!-- <br/><img src='/images/teleop.gif'> -->
<br/><img src='/images/g1_dance.gif'>

## Technical Contributions

1. **High-Level Arm Controller**:
   - Gesture switching (`DEFAULT`, `GRIP`, `RELEASE`) with Dex3 torque and position control.
   - File-based trajectory bank for quick replay in both joint and workspace modes.

2. **Whole-Body Motion Deployment**:
   - ONNX runtime inference for policies exported from IsaacGym.
   - Multi-policy control with remote button mapping (`L1`/`R1` for policy cycling, auto-return to stance).

3. **Safety Mechanisms**:
   - Zero-torque → damping → execution sequence.
   - Automatic abort on excessive torque, velocity, or invalid actions.
   - Fallback damping mode on emergency stop.

4. **Vision & Teleoperation**:
   - Real-time QR code detection for remote-triggered actions.
   - Gamepad-controlled operation for safe, interactive testing.

---
<br/><img src='/images/teleop.gif'>

## Impact

Enabled STARBOT INC to **deploy complex locomotion and manipulation behaviors** on the Unitree G1 with robust safety checks, smooth teleoperation, and efficient switching between motion policies — reducing operator intervention and improving development speed.

---
**Robot Github**: https://github.com/yifeichen2024/G1_deploy/tree/main
