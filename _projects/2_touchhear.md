---
layout: page
title: TouchHear
description: An AR assistive learning system that turns printed images into touch-responsive audio surfaces for visually impaired learners
img: assets/img/touchhear.jpg
importance: 5
category: lab
discuss_comments: false
translation: /zh/projects/2_touchhear/
---

**Sole developer** · Sep. 2025 – Dec. 2025

TouchHear lets a visually impaired student explore a printed image — a map, a diagram, a tactile figure — by touch, and hear an explanation of whatever region their finger is on. It was built for a study on teaching spatial and topographic concepts to visually impaired students.

## The problem

In the original study protocol, the "system" was a person: a researcher sat beside the participant, watched where their hand was on the tactile sheet, and played the matching audio by hand. This made sessions labor-intensive, made the timing of feedback depend on the researcher's attention, and meant the materials could not be used without a trained experimenter present.

TouchHear replaces that experimenter-in-the-loop step with real-time fingertip tracking, so the sheet responds on its own.

## How it works

TouchHear has two modes: one for teachers who prepare materials, and one for students who use them.

**1. Authoring (for teachers and researchers).**
A teacher loads any background image, draws rectangular regions on it, and assigns an audio clip to each region. No programming is needed. The tool then exports a printable A4 template with ArUco markers around the edges.

**2. Detection (for students).**
The printed sheet is placed under an Orbbec Femto Bolt RGB-D camera, and the system:

1. **Calibrates** — detects the ArUco markers and uses the depth image to fit the plane of the paper.
2. **Identifies the project** — the same markers encode which project the sheet belongs to, so the right regions and audio load automatically when a sheet is placed.
3. **Tracks the fingertip** — MediaPipe follows the index fingertip, and the depth camera measures its height above the paper; a touch is registered only when the fingertip is within 25 mm of the surface, so hovering does not trigger audio.
4. **Maps and plays** — the fingertip position is transformed from camera pixels into template coordinates, matched to a region, and the region's audio plays.

A design decision I like: the ArUco markers do double duty. One printed element handles both geometric calibration and project identity, which makes every sheet self-describing — there is no separate step to tell the system which material is in use.

## Implementation

- **Desktop client:** Python with PyQt6, structured as MVVM; the detection pipeline is split into calibration, project tracking, touch handling, coordinate mapping, and audio modules, connected through Qt signals.
- **Server:** FastAPI and PostgreSQL for accounts, project storage, file uploads, and template generation, so materials made on one machine can be synced to another.
- **Deployment:** Docker Compose.
