---
title: "Learning Nonlinear Dynamics and Control for an Unbalanced Disk"
date: 2026-06-13
weight: 30
summary: "Learning dynamics and control policies for an unbalanced disk-pendulum setup."
tags:
  - control
  - machine-learning
  - reinforcement-learning
  - featured
authors:
  - me
tech_stack:
  - Python
  - Gaussian Processes
  - Sparse GP
  - SAC
  - PPO
  - DQN
  - DDPG
links:
  - type: custom
    url: report.pdf
    label: Final report
    icon: document-text
featured: true
status: "Private code"
role: "Learning-based control project"
gallery:
  - type: video
    src: media/unbalanced-disk-demo.mp4
    mime: video/mp4
    caption: Short project clip associated with the unbalanced-disk learning and control experiments.
---

## Overview

Course project on learning dynamics and controllers for an unbalanced disk-pendulum setup. We compared model identification and reinforcement-learning approaches for swing-up and stabilization.

{{< project-gallery >}}

## Methods

- GP and sparse-GP dynamics models.
- ANN-based model identification.
- SAC, PPO, DQN, and custom DDPG control experiments.
- Real setup testing with the unbalanced disk hardware.

## What I Learned

- A clean one-step model fit does not automatically produce stable control.
- State representation and normalization can matter as much as the algorithm.
- The hardware setup exposes reset, saturation, and timing issues that simulation can hide.

## Report

The final report is available as a local PDF: [Machine Learning for Systems and Control report](report.pdf).
