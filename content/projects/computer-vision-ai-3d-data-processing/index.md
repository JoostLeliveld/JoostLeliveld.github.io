---
title: "Computer Vision AI and 3D Data Processing"
date: 2026-06-18
weight: 50
summary: "Three TU/e computer-vision projects: neural networks, point clouds, and autoencoders."
aliases:
  - /projects/computer-vision-ai-3d-data-analysis/
tags:
  - computer-vision
  - machine-learning
  - ros
  - 3d-data
  - featured
authors:
  - me
tech_stack:
  - Python
  - ROS
  - Point Clouds
  - Neural Networks
  - Autoencoders
  - Computer Vision
# Root-absolute paths: the portfolio/collection blocks resolve relative link
# URLs against the site root, so `neural-networks.pdf` would 404 on the cards.
links:
  - type: custom
    url: /projects/computer-vision-ai-3d-data-processing/neural-networks.pdf
    label: Neural networks report
    icon: document-text
  - type: custom
    url: /projects/computer-vision-ai-3d-data-processing/point-cloud-filtering.pdf
    label: Point-cloud filtering report
    icon: document-text
  - type: custom
    url: /projects/computer-vision-ai-3d-data-processing/autoencoder-anomaly-detection.pdf
    label: Autoencoder anomaly report
    icon: document-text
featured: true
status: "Course reports"
role: "Computer vision coursework"
gallery:
  - type: image
    src: featured.png
    alt: Unfiltered and filtered point-cloud views
    caption: Point-cloud filtering project showing unfiltered and filtered 3D views.
---

## Overview

Three projects from the TU/e Computer Vision AI and 3D Data Processing course. The work moves from neural-network basics to robot-facing 3D perception and autoencoder-based anomaly detection.

{{< project-gallery >}}

## Reports

- [Fundamentals of neural networks](neural-networks.pdf)
- [3D point cloud filtering](point-cloud-filtering.pdf)
- [Anomaly detection with autoencoder](autoencoder-anomaly-detection.pdf)

## Topics Covered

| Report | Focus |
| --- | --- |
| Neural networks | MLPs, segmentation losses, focal loss, precision, and recall. |
| Point clouds | Stereo-camera point-cloud generation, noise sources, and ROS filtering. |
| Autoencoders | Denoising, reconstruction error, thresholding, ROC/AUC, and false alarms. |

## What I Learned

- Representation choices shape what a vision model can learn.
- Point clouds make sensor noise and filtering decisions very visible.
- Anomaly detection depends on evaluation and thresholds, not only architecture.
