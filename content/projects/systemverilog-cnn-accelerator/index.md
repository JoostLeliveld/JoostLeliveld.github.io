---
title: "CNN Accelerator in SystemVerilog"
date: 2026-06-11
weight: 50
summary: "Embedded AI systems project focused on weight reuse, simulation, verification, and hardware-oriented neural-network execution."
tags:
  - ai-systems
  - embedded-ai
  - systemverilog
  - featured
authors:
  - me
tech_stack:
  - SystemVerilog
  - Digital Design
  - CNNs
  - Simulation
  - Verification
links: []
featured: true
status: "Portfolio summary"
role: "Embedded AI project"
---

## Overview

This project is less central to the robotics story, but it is useful for AI-systems and embedded-computing roles. It focuses on implementing and verifying a CNN accelerator in SystemVerilog, with attention to data movement, reuse, simulation, and correctness.

![SystemVerilog CNN accelerator datapath](datapath-diagram.svg)

## Engineering Focus

The portfolio angle is not the course lab itself. The interesting engineering story is:

- Weight-reuse dataflow for convolutional computation.
- Memory and compute organization for neural-network layers.
- Simulation-driven verification of datapath behavior.
- Testbench design and result checking.
- Trade-offs between hardware structure, throughput, and implementation complexity.

## Result Evidence To Publish

A strong public writeup would include:

- Block diagram of the accelerator datapath.
- Explanation of the weight-reuse strategy.
- Simulation waveform screenshots.
- Verification table for representative layers or kernels.
- Resource/timing notes if available.

| Evidence type | What it should demonstrate |
| --- | --- |
| Datapath diagram | How input tiles, weights, MACs, accumulation, and output buffers connect |
| Waveform screenshot | Valid/ready behavior and expected output timing in simulation |
| Verification table | Representative kernels or layers checked against reference outputs |
| Resource note | Hardware trade-offs around reuse, buffering, and throughput |

## Why It Belongs Here

Most of my portfolio focuses on robotics software, perception, and learning. This project broadens that story toward embedded AI and semiconductor-facing engineering: how learned models can be mapped toward hardware execution rather than only trained or simulated in Python.

## Source Availability

The source is not currently published. This page is designed as a high-level case study for roles where AI systems, embedded compute, or hardware/software boundaries matter.
