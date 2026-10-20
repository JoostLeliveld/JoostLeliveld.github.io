---
title: "Visibility-Aware Navigation from External Cameras"
date: 2026-06-15
weight: 10
summary: "MSc thesis: a warehouse robot that navigates with fixed wall cameras and plans around their blind spots."
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
status: "Completed (Oct 2026)"
role: "MSc Graduation Project (9/10)"
gallery:
  - type: image
    src: featured.png
    alt: Gazebo warehouse scene viewed from one of the wall cameras
    caption: The simulated warehouse as one wall camera sees it. The robot is the small marker on the right. The shelving hides parts of the floor, which is what the camera accuracy model has to capture.
---

## Overview

My MSc graduation project at BIASlab, TU/e. A mobile robot in a simulated warehouse is localized by five fixed wall cameras instead of its own sensors. How well a camera sees the robot depends on distance, viewing angle and what is in the way, so I learned where each camera can be trusted and used that in both localization and route planning.

Thesis: [Camera-Network Modelling for Belief-Space Robot Navigation](/publications/external-camera-robot-navigation/) (graded 9/10). Paper: [IWAI 2026](/publications/iwai2026-efe-camera-reliability/).

{{< project-gallery >}}

{{< project-video src="/publications/external-camera-robot-navigation/thesis_video.mp4" mime="video/mp4" caption="One-minute overview made from the recorded Gazebo runs." >}}

## What I Built

- A ROS 2 and Gazebo warehouse simulation with five wall cameras and a TurtleBot3.
- A YOLO detector that finds the robot in each camera image, and a calibrated mapping from image to floor position.
- Gaussian Process models of how accurate each camera is across the floor.
- Camera fusion in an EKF, weighted by those accuracy models.
- An Expected Free Energy route planner in CasADi that prefers routes where the cameras can track the robot.
- A reproducible pipeline: dataset capture, detector training, model fitting and seeded test campaigns.

## Result

In the paper's 40-run Gazebo campaign, the planner with the learned camera model reached all 20 goals without leaving the driving area. The planner that assumes the same camera accuracy everywhere reached 15 of 20 and left the driving area in the other five, all on the task with poor camera coverage. In the thesis, the learned model also kept the robot on track when one camera was switched off. All results are from simulation.
