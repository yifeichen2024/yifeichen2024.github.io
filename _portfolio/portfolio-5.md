---
title: "Simulation Deployment for Bi-Manual Dexterous Teleoperation System"
excerpt: "Built simulation environments in Drake, MuJoCo, and Genesis to enable teleoperation and policy training for a high-DOF humanoid manipulation platform.<br/><img src='/images/dexnex-drake.png'>"
collection: portfolio
---

This project supports the development of autonomous dexterous manipulation policies by enabling full-stack simulation of the **DexNex platform** — a bi-manual robot with Shadow Dexterous Hands — across multiple simulators including **Drake**, **MuJoCo**, and **Genesis**.

📍 **Affiliation**: HAND Engineering Research Center, Northwestern University  
🔧 **Role**: Simulation Engineer (System Integration)  
🔬 **Keywords**: teleoperation, dexterous hands, simulation, Drake, MuJoCo, Genesis, policy training

## Highlights

- 🛠️ **System**: DexNex includes dual ABB GoFa arms, Shadow Hands with 35 controllable joints, and full tactile and visual sensing.
- 🎮 **Goal**: Reconstruct the entire system in simulation to support teleoperation, demonstration collection, and diffusion policy learning.
- 🌐 **Multi-Sim Deployment**:
  - Built high-fidelity kinematic and dynamic models in **Drake**, matching physical behavior for remote control.
  - Ported the system to **MuJoCo** for high-speed RL experimentation and contact-rich manipulation.
  - Extended compatibility to **Genesis** for visual realism and future sim2real validation.

## Key Results

- 🧪 Enabled real-time teleoperation in Drake, improving feedback alignment and training data quality.
- 🔁 Cross-simulator consistency allows for policy benchmarking under different dynamics and rendering conditions.
- 🚀 Accelerated experimentation by reducing setup effort for downstream ML training and hardware integration.

**Robot Model**: https://github.com/yifeichen2024/avater_drake

![DexNex Sim View](/images/dexnex-drake.png)
*Figure: Simulated DexNex system with dual arms and dexterous hands in a manipulation task.*

![DexNex Sim View](/images/dexnex_real.png)
*Figure: Me with DexNex system with dual arms and dexterous hands.*