---
title: "In-Hand Manipulation with Enforced Grasp Stability"
excerpt: "Embedding force closure and torque sensing into RL for contact-rich manipulation.<br/><img src='/images/inhand_timelapse.png'>"
collection: portfolio
---

This work proposes a novel reinforcement learning pipeline that embeds **force/torque sensing** and **force-closure-based rewards** into in-hand manipulation training, significantly improving **grasp stability** and **policy convergence**.

📍 **Presented at**: ICRA 2025 Workshop — Learning Meets Model-Based Methods for Contact-Rich Manipulation  
✍️ **Authors**: Yifei Chen\*, Shihan Lu\*, Haoxuan Zhang, Kevin M. Lynch  
🔬 **Keywords**: dexterous manipulation, force closure, RL, grasp stability, contact-rich tasks

## Highlights

- 💡 **Problem**: Existing in-hand policies often lack true grasp stability, relying on palm support or precarious fingertip balancing.
- 🧠 **Solution**: Introduce force/torque readings at fingertips into the observation space and design a reward encouraging **multi-finger contact** and **force closure**.
- 🔬 **Method**:  
  - SAC agent learns to rotate a cube in-hand using a palm-down Allegro Hand in MuJoCo.  
  - Grasp stability is quantified using SVD over the grasp wrench matrix.  
  - RL reward combines rotation progress, object drop penalty, and contact quality.

## Key Results

- 🚀 With FC reward and F/T sensing, episode duration and stability improve significantly.
- 🧪 Robustness maintained even under randomized initial cube states.
- 🎯 Clear trade-off learned between in-hand rotation and grasp security.

![Training Curve](/images/inhand_reward_curve.png)
*Figure: Comparison of average reward during training with and without force-closure reward.*

![Manipulation Sequence](/images/inhand_timelapse.png)
*Figure: Manipulation time-lapse. FC policy maintains better contact during spinning.*

