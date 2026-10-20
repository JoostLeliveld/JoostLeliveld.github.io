---
title: "Camera-Network Modelling for Belief-Space Robot Navigation"
authors:
  - Joost Leliveld
date: 2026-10-06
doi: ""
publication_types:
  - thesis
publication: "MSc thesis, Eindhoven University of Technology (graded 9/10; MSc awarded cum laude)"
publication_short: "MSc thesis, TU/e"
abstract: |
  Fixed external cameras can localise a mobile robot without onboard perception, but the accuracy of their measurements depends on the robot position relative to the cameras and to the objects that block their view. We learn a measurement model from camera measurements paired with reference poses in a simulated warehouse. A learned correction removes the systematic displacement of the measured positions and global, per-camera and spatial covariance models describe the remaining error. The covariance models weight camera measurements in fusion and predict the expected camera information along routes in an expected-free-energy planner. On held-out data, spatial covariance weighting reduces the fused position error by 34.7% relative to equal weighting. In the final 90-run closed-loop campaign, the spatial model completes 15 of 15 runs both with the intact network and with one camera dropped, without entering a no-go region.
summary: "MSc thesis (9/10) on learning camera-network measurement models for belief-space navigation. Supervisors: Dr. W.M. Kouw and Dr. Ö. Arslan (BIASlab, TU/e)."
tags:
  - robotics
  - computer-vision
  - sensor-fusion
  - autonomous-navigation
featured: true
url_pdf: ""
url_slides: ""
url_video: ""
links:
  - type: code
    url: https://github.com/JoostLeliveld/UnembodiedNavigation
    label: Code
  - type: custom
    url: /projects/external-camera-robot-navigation/
    label: Project page
---

MSc thesis at BIASlab, Eindhoven University of Technology, supervised by Dr. W.M. Kouw and Dr. Ö. Arslan. Defended on 6 October 2026, graded 9/10.

{{< project-video src="thesis_video.mp4" mime="video/mp4" caption="One-minute overview of the thesis, made from the recorded Gazebo simulation runs: five wall cameras, YOLO detection, learned camera accuracy maps, and route choice when a camera fails." >}}

This page gives a public summary; the full thesis is not published. A companion paper is in preparation. Related: the [IWAI 2026 paper](/publications/iwai2026-efe-camera-reliability/).
