---
title: "Final Report Machine Learning for Systems and Control"
authors:
  - Joost Leliveld
  - Project team
date: 2026-06-18
doi: ""
publication_types:
  - report
publication: "Machine Learning for Systems and Control course report, Eindhoven University of Technology"
publication_short: "MLSC report"
abstract: |
  This report studies data-driven dynamics identification and policy learning for an unbalanced disk-pendulum setup. It combines Gaussian Process and neural-network model identification with reinforcement-learning approaches for swing-up and stabilization control.
summary: "Course report on GP/ANN system identification and reinforcement learning for an unbalanced disk-pendulum."
tags:
  - control
  - reinforcement-learning
  - gaussian-processes
featured: false
links:
  - type: pdf
    url: /projects/learning-unbalanced-disk-control/report.pdf
    label: Report PDF
  - type: custom
    url: /projects/learning-unbalanced-disk-control/
    label: Project page
---

## What the report covers

The unbalanced disk is a small pendulum-like setup that is easy to describe and hard to control well: it is nonlinear, it saturates, and swing-up needs energy the controller cannot apply directly.

The report works through two halves of that problem. The first identifies the dynamics from measured data, comparing Gaussian Process and sparse-GP models against a neural-network model and looking at where a good one-step prediction stops being a good multi-step one. The second learns controllers — SAC, PPO, DQN, and a custom DDPG — for swing-up and stabilization, then runs them on the real hardware.

The most useful part is the gap between the two: model fits that look clean in isolation did not automatically produce stable control, and state representation and normalization mattered as much as the choice of algorithm.
