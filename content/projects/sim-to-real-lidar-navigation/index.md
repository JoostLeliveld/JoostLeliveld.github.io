---
title: "Sim-to-Real LiDAR Navigation for the Origin One Robot"
date: 2026-06-14
weight: 20
summary: "Isaac Lab reinforcement learning for LiDAR-based Origin One navigation."
tags:
  - robotics
  - reinforcement-learning
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
    label: WheeledLab (upstream project we built on)
    icon: link
featured: true
status: "Team project"
role: "Team project"
gallery:
  - type: image
    src: featured.jpeg
    alt: Origin One robot in a lab obstacle course
    caption: Origin One in the lab environment used for navigation and obstacle-avoidance testing.
---

## Overview

Team internship project on LiDAR-based mobile robot navigation for the Origin One platform. We trained PPO policies in Isaac Lab/Isaac Sim and worked on the interfaces needed to move from simulation toward ROS/Gazebo and the real robot.

{{< project-gallery >}}

## What I Worked On

- LiDAR observation and goal-relative state design.
- Differential-drive action interface for Origin One.
- PPO reward and curriculum configuration.
- Training infrastructure and integration with the Origin-oriented WheeledLab foundation.

## What I Learned

- Sim-to-real work is mostly interface discipline: observations, actions, frames, and control assumptions all have to survive the jump between tools.
- A policy is only one part of the system; training setup, export path, and robot constraints shape whether it is usable.
