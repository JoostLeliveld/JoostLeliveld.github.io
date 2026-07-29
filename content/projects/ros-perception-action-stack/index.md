---
title: "ROS Perception-to-Action Jetson RC Car"
date: 2026-06-12
weight: 40
summary: "Jetson RC car stack connecting vision, target tracking, obstacle avoidance, and robot motion."
tags:
  - robotics
  - computer-vision
  - ros
  - embedded-control
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
links:
  - type: custom
    url: /projects/ros-perception-action-stack/report.pdf
    label: Embedded Visual Control report
    icon: document-text
featured: true
status: "Project note"
role: "Robotics software integration"
gallery:
  - type: video
    src: media/jetson-rc-car-demo.mp4
    poster: featured.jpg
    mime: video/mp4
    caption: Jetson-based RC car used for the person identification, tracking, and following stack.
  - type: image
    src: media/ros-architecture.png
    alt: Implemented ROS architecture for person identification, tracking, and following
    caption: ROS architecture with vision, identification, tracking, obstacle avoidance, state management, and motion control.
---

## Overview

Embedded Visual Control project on a Jetson-based RC car. The stack turns camera observations into behavior by combining person detection, identification, tracking, obstacle avoidance, state management, and motor control.

{{< project-gallery >}}

## What It Shows

| Layer | What matters |
| --- | --- |
| Perception | Camera stream, person detection, and identification |
| Behavior | Search, track, follow, and avoid-obstacle states |
| Control | Motion commands connected to feedback and safety logic |
| ROS glue | Topics and node boundaries that make the system debuggable |

## What I Learned

- Integration is its own engineering problem; a good detector is not enough.
- ROS boundaries help only when topics, frames, and node responsibilities stay simple.

## Report

The report is available as a local PDF: [Person Identification, Tracking and Following](report.pdf).
