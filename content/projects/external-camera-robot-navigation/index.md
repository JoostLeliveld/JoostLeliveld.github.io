---
title: "External-Camera Robot Navigation"
date: 2026-06-15
summary: "A graduation project on mobile robot navigation from external camera observations, combining geometric perception, state estimation, and learning-based control."
tags:
  - Robotics
  - Computer Vision
  - Sensor Fusion
  - Autonomous Navigation
  - Learning-Based Control
authors:
  - me
tech_stack:
  - Python
  - ROS 2
  - Gazebo
  - OpenCV
  - NumPy
  - SciPy
links:
  - type: github
    url: https://github.com/JoostLeliveld
    label: GitHub
featured: true
status: "In progress"
role: "Graduation Project"
---

## Overview

This graduation project investigates mobile robot navigation using an external fixed camera instead of relying only on onboard sensing. The system combines geometric computer vision, robot state estimation, and learning-based planning/control to navigate a mobile robot from start to goal using externally observed sensing.

The core question is how camera geometry, visibility, and sensor reliability should influence autonomous navigation decisions. I use simulation and robotics tooling to evaluate navigation behavior in controlled environments before moving toward more realistic deployment constraints.

## Why This Project

External cameras can provide a useful global view of a robot and its environment, but they also introduce their own problems: perspective distortion, occlusion, calibration errors, and uncertainty about what the camera can reliably observe. This project is about making those constraints explicit instead of treating perception as a perfect input to the planner.

## What I Am Building

The pipeline connects camera projection models, homography-based localization, robot dynamics, planning/control, and experiment logging. The goal is to make it easy to compare navigation behavior under different camera viewpoints, visibility assumptions, and sensing reliability settings.

## Highlights

- Developed an external-camera navigation setup for a mobile robot using projection geometry and planar homography.
- Combined robot dynamics, perception, and planning/control into a reproducible experimental pipeline.
- Investigated how camera viewpoint, visibility, and sensing reliability affect navigation performance.
- Designed experiments around autonomous navigation, sensor fusion, and real-world robotic constraints.

## Tech

The project is implemented mainly in Python and ROS 2, with simulation support through Gazebo. Computer vision components use camera projection models, homography-based localization, and image-space robot observations. The planning and evaluation pipeline combines robot dynamics, state estimation, and learning-based control methods.

## Links

- [GitHub profile](https://github.com/JoostLeliveld)
