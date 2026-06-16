---
title: "Sim-to-Real LiDAR Navigation for the Origin One Robot"
date: 2026-06-14
weight: 20
summary: "Team internship project using Isaac Lab reinforcement learning for LiDAR-based Origin One navigation."
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
status: "Team project"
role: "Team project"
gallery: []
---

## Overview

This team internship project demonstrates an end-to-end sim-to-real workflow for LiDAR-based mobile robot navigation using reinforcement learning. The public repository targets the Origin One platform and builds on Isaac Lab/Isaac Sim tooling for training, assets, environments, and reinforcement-learning workflows.

![Project overview](featured.png)

![Navigation environment](navigation-environment.png)

{{< project-gallery >}}

## System

The project trains an Origin One robot to navigate from a starting position to a final goal while avoiding obstacles. The public training entry point is:

```bash
python source/avulab_rl/scripts/train_rl.py --headless -r RSS_NAV_CONFIG
```

The repository uses Weights & Biases for training logs and videos, and documents an Isaac Lab setup with custom packages for assets, tasks, and RL code.

![Observation and action design](observation-action.svg)

## RL Interface

The public-facing interface is a LiDAR navigation policy: range observations and goal-relative state feed a PPO policy, which outputs differential-drive velocity commands. The reward design is organized around progress to the goal, collision avoidance, control smoothness, and task completion.

| Interface piece | Project summary |
| --- | --- |
| Observation | LiDAR geometry plus goal-relative navigation state |
| Action | Differential-drive command for the Origin One platform |
| Policy | PPO policy trained in Isaac Lab/Isaac Sim workflows |
| Transfer path | Policy export toward ROS 2, Gazebo, and real-world deployment tooling |

## What I Worked On

My work sat in the engineering layer of the project:

- Observation and action design for LiDAR-based navigation.
- Differential-drive control and Origin One platform integration.
- Curriculum and reinforcement-learning configuration work.
- Training infrastructure for the navigation task.
- Integration work connecting the project to the Origin-oriented WheeledLab foundation.

## What I Learned

- Sim-to-real work is mostly interface discipline: observations, actions, coordinate frames, and control assumptions all have to survive the jump between tools.
- A policy is only one part of the system. Training setup, export path, ROS/Gazebo integration, and robot constraints shape whether it is actually usable.
- Reward design is less about finding one clever term and more about making progress, safety, and smoothness pull in compatible directions.

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

## Current Artifacts

This page includes the public workflow figure, Isaac Lab navigation environment, and observation/action design diagram. Training videos, deployment clips, training curves, and final success-rate tables can be added later if the team material is cleared for sharing.

## Relation To My Other Work

This project complements my thesis work: the thesis emphasizes external-camera perception and uncertainty-aware planning, while this project emphasizes onboard LiDAR, reinforcement learning, and sim-to-real deployment on a physical mobile robot platform.
