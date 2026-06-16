---
title: "Learning Nonlinear Dynamics and Control for an Unbalanced Disk"
date: 2026-06-13
weight: 30
summary: "Nonlinear dynamics and control project using Gaussian Processes and actor-critic reinforcement learning."
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
links: []
featured: true
status: "Private code"
role: "Learning-based control project"
---

## Overview

This project explored learning-based control for an unbalanced disk: a nonlinear dynamical system where the controller must reason about unstable behavior, state representation, model uncertainty, and the trade-off between learned dynamics and learned policies.

The repository is not public, so this page shows the system, methods, and lessons without exposing coursework code.

![Unbalanced disk learning-control summary](control-summary.svg)

## Engineering Question

How well can learned models and learned controllers handle a nonlinear mechanical system when the state representation, normalization, and model class strongly influence stability and control performance?

## Methods

- Nonlinear system identification from measured or simulated trajectories.
- Gaussian Process and sparse Gaussian Process dynamics models.
- Actor-critic reinforcement-learning controllers.
- SAC, PPO, DQN, and a custom DDPG implementation.
- State encoding, normalization, and quantitative comparisons across model/control choices.

## What I Looked For

| Evidence type | What it demonstrates |
| --- | --- |
| Rollout plot | Learned dynamics versus measured or simulated trajectories |
| Reward curve | Convergence and stability differences across SAC, PPO, DQN, and DDPG |
| Failure table | Which methods were sensitive to state encoding, scaling, or exploration |
| Control metric | Tracking, stabilization, or energy-use comparison on held-out rollouts |

## What I Learned

- Model quality and controller quality are coupled; a clean rollout fit does not automatically mean stable control.
- State representation and normalization can dominate the result as much as the learning algorithm.
- Comparing several controllers is useful because each failure mode teaches something different about the system.

## Notes

Source code is private for now. A cleaned repository becomes useful once the experiment scripts, report figures, and reproducible results are separated from coursework scaffolding.
