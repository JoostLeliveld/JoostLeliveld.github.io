---
title: "Visibility-Aware Navigation from External Cameras"
date: 2026-06-15
weight: 10
summary: "External-camera robot navigation with visibility-aware planning uncertainty."
tags:
  - robotics
  - computer-vision
  - sensor-fusion
  - autonomous-navigation
  - learning-based-control
  - featured
authors:
  - me
tech_stack:
  - Python
  - ROS 2
  - Gazebo
  - YOLO
  - Gaussian Processes
  - Expected Free Energy
  - NumPy
  - SciPy
links:
  - type: github
    url: https://github.com/JoostLeliveld/UnembodiedNavigation
    label: Repository
featured: true
status: "In progress"
role: "Graduation Project"
gallery: []
---

## Overview

This graduation project studies mobile robot navigation from a fixed external camera. I use Gazebo, YOLO-based robot detection, BEV state estimation, and a Gaussian Process reliability model so the planner can account for where camera observations are likely to fail.

{{< project-gallery >}}

## What I Built

- ROS/Gazebo stack for external-camera localization and robot navigation.
- Detector-to-pixel observation pipeline with BEV state estimation.
- GP reliability map used as state-dependent camera covariance.
- Seeded warehouse benchmark comparing constant and visibility-aware covariance.

## Result Snapshot

| Condition | Planner | Clean reaches | Collisions | Other outcomes |
| --- | --- | ---: | ---: | --- |
| C1 | constant camera covariance | 12/20 | 8/20 | none |
| C2 | visibility-aware covariance | 16/20 | 2/20 | 1 near-success, 1 infrastructure-invalid |

## Takeaway

Perception quality becomes a planning variable once it affects state uncertainty. The interesting part is not just detecting the robot, but making the planner honest about when the camera view is unreliable.
