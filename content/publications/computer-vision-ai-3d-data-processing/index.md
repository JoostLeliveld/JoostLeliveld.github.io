---
title: "Computer Vision AI and 3D Data Processing Reports"
authors:
  - Joost Leliveld
date: 2026-06-18
doi: ""
publication_types:
  - report
publication: "Computer Vision AI and 3D Data Processing coursework reports, Eindhoven University of Technology"
publication_short: "Computer vision reports"
aliases:
  - /publications/computer-vision-ai-3d-data-analysis/
abstract: |
  This collection covers three course projects on neural-network fundamentals, stereo-camera point-cloud filtering with ROS, and autoencoder-based anomaly detection. The reports connect model behavior, 3D perception, filtering, thresholding, and evaluation choices.
summary: "Course report collection covering neural networks, point-cloud filtering, and autoencoder anomaly detection."
tags:
  - computer-vision
  - 3d-data
  - machine-learning
featured: false
links:
  - type: pdf
    url: /projects/computer-vision-ai-3d-data-processing/point-cloud-filtering.pdf
    label: Point-cloud filtering report
  - type: custom
    url: /projects/computer-vision-ai-3d-data-processing/neural-networks.pdf
    label: Neural networks report
  - type: custom
    url: /projects/computer-vision-ai-3d-data-processing/autoencoder-anomaly-detection.pdf
    label: Autoencoder anomaly report
  - type: custom
    url: /projects/computer-vision-ai-3d-data-processing/
    label: Project page
---

## What the reports cover

Three separate reports, moving from 2D model behavior toward robot-facing 3D perception.

The **neural networks** report works through MLPs and segmentation losses, including why focal loss helps on imbalanced data and how precision and recall move against each other as the threshold changes.

The **point cloud** report generates point clouds from a stereo camera and filters them in ROS. It is the most sensor-honest of the three: noise sources, dropout, and the trade-off between filtering aggressively and deleting real structure are all visible in the output.

The **autoencoder** report uses reconstruction error for anomaly detection, with denoising, threshold selection, and ROC/AUC evaluation. The conclusion is that the architecture mattered less than where the threshold was placed and what a false alarm actually costs.
