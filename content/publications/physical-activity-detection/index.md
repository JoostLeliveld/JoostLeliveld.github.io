---
title: "Physical Activity Detection in Elderly Diabetes Patients Using Raw Smartwatch Data"
authors:
  - Joost Leliveld
date: 2023-06-30
doi: ""
publication_types:
  - report
publication: "Bachelor End Project report, Eindhoven University of Technology"
publication_short: "Bachelor End Project"
abstract: |
  This Bachelor End Project investigated physical-activity detection from raw wrist-worn smartwatch accelerometer data in elderly diabetes patients. Hidden Markov Models were compared with self-reported activities and a traditional cut-points approach, with attention to recall, overestimation, and participant-level variation.
summary: "Bachelor End Project report on unsupervised physical-activity detection from raw smartwatch data."
tags:
  - machine-learning
  - signal-processing
  - wearable-sensing
featured: false
links:
  - type: pdf
    url: /projects/physical-activity-detection/report.pdf
    label: Report PDF
  - type: custom
    url: /projects/physical-activity-detection/
    label: Project page
---

## What the report covers

Free-living accelerometer data from elderly diabetes patients is noisy, unlabeled, and collected without a researcher watching. The report asks whether Hidden Markov Models can recover activity states from it better than the cut-points method commonly used in the field.

It covers feature extraction from raw accelerometer and orientation signals, the smoothing and preprocessing that noisy wrist-worn data needs, and patient-specific HMMs fitted per participant. Results are compared against both self-reported activity and a traditional cut-points baseline.

The honest finding is about evaluation rather than modeling: the HMM reached higher recall, but recall only means something once you understand how much the model overestimates, and participant-level variation was large enough that a single global threshold was never going to work.
