---
title: "Pathology Image Analysis"
date: 2021-01-15
weight: 90
summary: "Earlier computer-vision coursework on lesion analysis using color, asymmetry, border, and diameter features."
tags:
  - earlier-work
  - computer-vision
  - image-analysis
authors:
  - me
tech_stack:
  - Python
  - OpenCV
  - NumPy
  - Image Processing
links:
  - type: github
    url: https://github.com/merlijnvb/8QA01-Beeldanalyse-voor-Pathologie
    label: Team Repository
featured: false
status: "Earlier work"
role: "Team coursework"
---

## Overview

This is earlier computer-vision coursework around skin-lesion image analysis. The project explored whether an algorithm could assess melanoma-related visual features from an image using color, asymmetry, diameter, and border characteristics.

I keep this separate from the main robotics case studies because it is older and less aligned with my current portfolio direction, but it still shows useful early experience with image processing and feature engineering.

## Approach

The project followed the ABCD-style analysis idea:

- Asymmetry from blob overlap after flipping regions around the lesion center.
- Border features from contour extraction.
- Color-region scoring from thresholded masks.
- Diameter-related measurements from segmented lesion geometry.

## Why It Is Earlier Work

There are multiple related repositories from this period, so this page links only the clearest team-owned version rather than turning each repository into a separate portfolio card.

## What I Would Improve Today

If revisiting this project, I would consolidate the duplicated repositories, document the dataset and evaluation protocol more clearly, and separate exploratory scripts from a clean reproducible pipeline.
