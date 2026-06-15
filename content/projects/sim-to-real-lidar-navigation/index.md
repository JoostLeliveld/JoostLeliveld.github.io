---
title: "Sim-to-Real LiDAR Navigation for the Origin One Robot"
date: 2026-06-14
weight: 20
summary: "Team internship case study: Isaac Lab reinforcement learning for LiDAR-based Origin One navigation with sim-to-real deployment goals."
tags:
  - robotics
  - reinforcement-learning
  - sim-to-real
  - autonomous-navigation
  - featured
authors:
  - me
tech_stack:
  - Python
  - Isaac Lab
  - Isaac Sim
  - PPO
  - LiDAR
  - Gazebo
links:
  - type: github
    url: https://github.com/kgulikers/Team_internship_5ARIP10
    label: Team Repository
  - type: custom
    url: https://github.com/TUe-Ray/Wheeled-lab
    label: Related Origin Integration
    icon: link
featured: true
status: "Completed internship"
role: "Team project"
---

## Overview

This team internship project demonstrates an end-to-end sim-to-real workflow for LiDAR-based mobile robot navigation using reinforcement learning. The public repository targets the Origin One platform and builds on Isaac Lab/Isaac Sim tooling for training, assets, environments, and reinforcement-learning workflows.

![Project overview](https://raw.githubusercontent.com/kgulikers/Team_internship_5ARIP10/main/docs/media/Overview.png)

![Navigation environment](https://raw.githubusercontent.com/kgulikers/Team_internship_5ARIP10/main/docs/media/navigation_environment.png)

## System

The project trains an Origin One robot to navigate from a starting position to a final goal while avoiding obstacles. The public training entry point is:

```bash
python source/avulab_rl/scripts/train_rl.py --headless -r RSS_NAV_CONFIG
```

The repository uses Weights & Biases for training logs and videos, and documents an Isaac Lab setup with custom packages for assets, tasks, and RL code.

## My Contribution

My attributed work belongs in the core engineering layer, not only documentation. The portfolio-relevant contribution areas are:

- Observation and action design for LiDAR-based navigation.
- Differential-drive control and Origin One platform integration.
- Curriculum and reinforcement-learning configuration work.
- Training infrastructure for the navigation task.
- Integration work that connects the project to the Origin-oriented WheeledLab foundation.

## Public Evidence

The team repository citation names me as a co-author:

```bibtex
@misc{5ARIP10_2025,
  author = {Leliveld, Joost and Musat, Cristina and Huang, Shao-Ruei and Gulikers, Kevin},
  title  = {Demonstrating an End-to-End Sim-to-Real Transfer for Lidar-Based Navigation Using Reinforcement Learning},
  howpublished = {This repository},
  url = {https://github.com/kgulikers/Team_internship_5ARIP10},
}
```

## What I Would Show in a Demo

The strongest public version of this page would include the Isaac Lab training video, Gazebo or real-robot deployment video, observation/action-space diagrams, reward design, training curves, and a final success-rate table. The page is structured for those artifacts once they are ready to publish.

## Why It Matters

This project complements my thesis work: the thesis emphasizes external-camera perception and uncertainty-aware planning, while this project emphasizes onboard LiDAR, reinforcement learning, and sim-to-real deployment on a physical mobile robot platform.
