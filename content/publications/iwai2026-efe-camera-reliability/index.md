---
title: "Expected Free Energy Planning with Learned External-Camera Measurement Reliability"
authors:
  - Joost Leliveld
  - Ömür Arslan
  - Wouter M. Kouw
date: 2026-10-16
doi: ""
publication_types:
  - paper-conference
publication: "International Workshop on Active Inference (IWAI 2026), Springer (to appear)"
publication_short: "IWAI 2026, full paper"
abstract: |
  A robot planning under uncertainty must trade goal progress against whether it will be able to localize itself effectively at potential future positions. We study this problem in Gazebo simulation for a mobile robot localized by a fixed external camera, where detector reliability varies with viewpoint, occlusion, and position in the image. We fit a Gaussian process to the confidence scores of a trained object detector, giving a spatial estimate of detector reliability over the workspace, and use it as a state-dependent observation covariance in an Expected Free Energy planner. In a 40-run Gazebo campaign over four tasks and five seeds, the planner using this state-dependent covariance reaches all 20 goals without leaving the traversable region, while the uniform-covariance planner reaches 15/20 and leaves the region in the other five runs, all on the camera-poor task.
summary: "Peer-reviewed paper (IWAI 2026): learned camera reliability makes an active-inference planner pick routes where the robot stays localizable."
tags:
  - robotics
  - active-inference
  - gaussian-processes
  - autonomous-navigation
featured: true
url_pdf: "leliveld2026iwai_accepted.pdf"
url_code: "https://github.com/JoostLeliveld/iwai2026-camera-reliability-efe"
---

**Peer-reviewed full paper** at the International Workshop on Active Inference (IWAI 2026), presented as a talk and a poster on 16 October 2026. Leliveld, Arslan and Kouw, Eindhoven University of Technology.

[Download the paper (PDF)](leliveld2026iwai_accepted.pdf) · [Code on GitHub](https://github.com/JoostLeliveld/iwai2026-camera-reliability-efe) · [Related MSc thesis and video](/publications/external-camera-robot-navigation/)

The PDF is the accepted manuscript. The Version of Record will appear in the Springer proceedings. The DOI will be added here once it is published.
