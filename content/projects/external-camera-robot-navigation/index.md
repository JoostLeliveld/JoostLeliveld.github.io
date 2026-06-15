---
title: "Visibility-Aware Navigation from External Cameras"
date: 2026-06-15
weight: 10
summary: "Thesis flagship: external-camera robot navigation that turns learned detector reliability into state-dependent planning uncertainty."
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
  - type: custom
    url: https://github.com/JoostLeliveld/UnembodiedNavigation/tree/main/paper_artifacts
    label: Artifacts
    icon: document-chart-bar
featured: true
status: "In progress"
role: "Graduation Project"
---

## Overview

This graduation project investigates mobile robot navigation using a fixed external camera instead of relying only on onboard sensing. The system trains a detector in Gazebo, converts detector reliability into a spatial Gaussian Process, and uses that reliability as predictive camera covariance inside an expected-free-energy planner.

The core question is how camera geometry, visibility, and sensor reliability should influence autonomous navigation decisions before localization failure becomes a recovery problem.

![External-camera warehouse setup](https://raw.githubusercontent.com/JoostLeliveld/UnembodiedNavigation/main/paper_artifacts/figures/problem_setup_camera.png)

![External-camera navigation architecture](https://raw.githubusercontent.com/JoostLeliveld/UnembodiedNavigation/main/docs/media/system_architecture.svg)

## Why This Project

External cameras can provide a useful global view of a robot and its environment, but they also introduce perspective distortion, occlusion, calibration sensitivity, and spatially uneven detection quality. This project makes those constraints explicit instead of treating perception as a perfect input to the planner.

## System

The pipeline is:

```text
Gazebo warehouse
-> YOLO external-camera detector
-> image-space bottom-centre observation
-> BEV state estimate
-> GP reliability query
-> predictive camera covariance
-> EFE route planner
-> seeded campaign metrics
```

## Highlights

- Built a ROS/Gazebo external-camera navigation stack with detector-to-pixel observation, BEV state estimation, and planner integration.
- Trained and evaluated a simulated YOLO detector for robot localization under varying camera visibility.
- Fit a GP reliability model and used it to provide state-dependent camera covariance to the planner.
- Compared constant-covariance planning with visibility-aware planning in a seeded warehouse route-choice benchmark.

## Public Result Snapshot

The public repository reports a paper-facing benchmark with four warehouse tasks and five seeds per condition:

| Condition | Planner | Clean reaches | Collisions | Other outcomes |
| --- | --- | ---: | ---: | --- |
| C1 | constant camera covariance | 12/20 | 8/20 | none |
| C2 | visibility-aware covariance | 16/20 | 2/20 | 1 near-success, 1 infrastructure-invalid |

## Public Repository Structure

The repository is organized as a research artifact rather than just source code, with module pages for YOLO perception, GP covariance modeling, state estimation, EFE planning, experiments, figures, metrics, and reproduction commands.

Current release gaps noted in the repository are the overview video, license, citation metadata, and artifact/data availability statement.
