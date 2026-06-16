# Media Intake Guide

This site is now prepared for project images, plots, diagrams, and videos.

## Where To Put Files

Use each project as a Hugo page bundle. Put new assets under that project's `media/` folder:

```text
content/projects/external-camera-robot-navigation/media/
content/projects/sim-to-real-lidar-navigation/media/
content/projects/learning-unbalanced-disk-control/media/
content/projects/ros-perception-action-stack/media/
content/projects/systemverilog-cnn-accelerator/media/
content/projects/pathology-image-analysis/media/
content/outside/tennis-skiing/media/
```

Preferred names:

```text
overview-video.mp4
demo-run-01.mp4
training-curve.png
result-table.png
architecture.png
system-photo-01.jpg
waveform-01.png
tennis-serve-01.jpg
skiing-01.jpg
```

Keep originals outside the repo if they are huge. For the website, good targets are:

- Images: `.jpg`, `.png`, or `.webp`, ideally under 2500 px wide.
- Videos: `.mp4` or `.webm`, ideally 1080p or below and under about 50 MB each.
- Diagrams: `.svg` when they are clean vector diagrams, `.png` when exported from tools.

## Add A Gallery To A Project

Each project page has `gallery: []` in front matter and a `project-gallery` shortcode already placed in the page. To show assets, replace the empty gallery with entries like:

```yaml
gallery:
  - type: image
    src: media/training-curve.png
    alt: PPO training curve for the Origin One navigation policy
    caption: Training reward curve from the LiDAR navigation task.
  - type: video
    src: media/deployment-demo.mp4
    poster: media/deployment-demo-poster.jpg
    mime: video/mp4
    caption: Short deployment run showing the policy driving the robot toward a goal.
```

The gallery renders only when entries exist, so empty pages stay clean.

## Add A Single Video

For one important clip, use:

```md
{{< project-video src="media/overview-video.mp4" poster="media/overview-poster.jpg" mime="video/mp4" caption="One-minute overview of the external-camera navigation stack." >}}
```

## What To Send Later

For each asset, the useful input is:

```text
Project:
File name:
What it shows:
Where it belongs on the page:
Caption:
Can this be public? yes/no
People visible? yes/no
Contains private code/data? yes/no
```

## Best Missing Material

Highest impact:

- Thesis: overview video, route-choice plot, detector/reliability heatmap, final architecture, result table.
- Origin One: Isaac Lab training video, Gazebo or real-robot clip, training curve, reward summary, final success table.
- ROS stack: short demo clip, robot photo, calibration view, node/topic diagram.
- Unbalanced disk: rollout plot, reward curves, comparison table, phase portrait or setup photo.
- SystemVerilog: waveform screenshot, datapath export, verification table, timing/resource notes.
- Pathology: example segmentation masks and feature outputs, only if dataset rights are clear.
- Outside: 4-8 strong tennis/skiing photos with short captions, kept as a light personal page rather than the main story.
