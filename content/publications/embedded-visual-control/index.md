---
title: "Person Identification, Tracking and Following"
authors:
  - Joost Leliveld
  - Project team
date: 2025-06-30
doi: ""
publication_types:
  - report
publication: "Embedded Visual Control group report, Eindhoven University of Technology"
publication_short: "Embedded Visual Control report"
abstract: |
  This group report describes an embedded visual-control system for person identification, tracking, and following. It covers vision detection and recognition, tracking and following behavior, obstacle detection, motion control, state management, and integrated verification.
summary: "Embedded Visual Control report on person identification, tracking, following, and robot integration."
tags:
  - robotics
  - computer-vision
  - embedded-control
featured: false
links:
  - type: pdf
    url: /projects/ros-perception-action-stack/report.pdf
    label: Report PDF
  - type: custom
    url: /projects/ros-perception-action-stack/
    label: Project page
---

## What the report covers

A robot that follows a specific person has to do several things at once: detect people, decide which one is the target, keep that identity across frames, avoid obstacles while moving, and stop safely when any of the above fails.

The report documents that full stack on a Jetson-based RC car — vision detection and recognition, the tracking and following behavior, obstacle detection, motion control, and the state management that decides which behavior is active. It closes with integrated verification on the real vehicle.

Most of the engineering effort went into the boundaries rather than the components. A detector that works on a laptop still has to survive frame rates, latency, and a moving camera, and the state machine is what keeps those failures from becoming collisions.
