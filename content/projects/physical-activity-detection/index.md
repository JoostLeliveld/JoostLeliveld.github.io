---
title: "Smartwatch Activity Detection with Hidden Markov Models"
date: 2023-06-30
weight: 80
summary: "Bachelor End Project on physical-activity detection from raw smartwatch data."
tags:
  - earlier-work
  - machine-learning
  - signal-processing
  - biomedical-engineering
  - data-science
authors:
  - me
tech_stack:
  - Python
  - Hidden Markov Models
  - Accelerometer Data
  - Signal Processing
  - Wearable Sensing
links:
  - type: custom
    url: report.pdf
    label: Bachelor thesis report
    icon: document-text
featured: false
status: "Bachelor End Project"
role: "Individual thesis project"
gallery:
  - type: image
    src: featured.png
    alt: Predicted daily physical-activity minutes across participants
    caption: Model comparisons for predicted daily physical-activity minutes across participants.
---

## Overview

Bachelor End Project on detecting physical activity from raw wrist-worn smartwatch data in elderly diabetes patients. I compared Hidden Markov Models with self-reported activity and a traditional cut-points approach.

{{< project-gallery >}}

## What I Built

- Feature extraction from accelerometer and orientation signals.
- Smoothing and preprocessing for noisy free-living data.
- Patient-specific Hidden Markov Models for activity-state detection.
- Comparison against self-reports and cut-points.

## What I Learned

- Wearable-sensor validation is just as hard as the modeling.
- Higher recall is useful only if overestimation is understood.
- Health-related ML needs careful claims and careful evaluation.

## Report

The report is available as a local PDF: [Physical activity detection in elderly diabetes patients using raw smartwatch data](report.pdf).
