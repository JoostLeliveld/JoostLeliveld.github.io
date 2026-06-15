---
title: "ROS Perception-to-Action Robot Stack"
date: 2026-06-12
weight: 40
summary: "Practical robotics integration project connecting camera perception, target estimation, behavior logic, motor control, and encoder feedback."
tags:
  - robotics
  - computer-vision
  - ros
  - systems-integration
  - featured
authors:
  - me
tech_stack:
  - ROS
  - Python
  - OpenCV
  - Camera Calibration
  - Encoder Feedback
  - Motor Control
links: []
featured: true
status: "Demo pending"
role: "Robotics software integration"
---

## Overview

This project represents the practical robotics side of my portfolio: connecting perception to action in a working robot software stack. The goal is not just to train or evaluate a model offline, but to make camera observations drive robot behavior through ROS nodes, control logic, and feedback from the hardware.

## System Shape

```text
Camera
-> calibration and image preprocessing
-> detection or gesture recognition
-> target estimate
-> behavior logic
-> motor command
-> encoder feedback
```

## Components

- Camera calibration and image-processing pipeline.
- Detection, tracking, or gesture-recognition logic.
- Target-estimation interface for downstream behavior.
- ROS nodes for perception, decision logic, and actuation.
- Encoder feedback for closing the loop between command and motion.
- Natural-language or high-level robot-command experiments where appropriate.

## My Contribution

The value of this project is integration. It shows that I can connect sensors, software modules, control commands, and feedback into a robot-facing system rather than stopping at a notebook or standalone model.

## What I Would Publish

Before making this a public repository, I would consolidate the ROS nodes, add a launch file, include a short demo video, and document the main message interfaces. A strong public version should make it easy to understand how camera information becomes robot motion.

## Source Availability

The code is not currently published as a clean standalone repository. This page intentionally shows the architecture and contribution without exposing private or messy development history.
