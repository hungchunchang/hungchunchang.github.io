---
layout: page
title: ECRobot
description: ECRobot (Empathy Cognition Robot) — an Intelligent Tutoring System with empathetic feedback design
img: assets/img/ecrobot.png
importance: 2
category: lab
related_publications: true
translation: /zh/projects/1_ecrobot/
---

**[GitHub](https://github.com/hungchunchang/EmpathyCognitiveRobot)**

**Sole developer** · Sep. 2025 – Dec. 2025  
_Enterprise Information Systems_, 2026; _Educational Psychology_, under revision

The ECRobot (Empathy Cognition Robot) project investigates the effect of empathetic design on intelligent tutoring systems (ITS). The system assists students in completing linguistic puzzles with LLM-generated, empathetic real-time feedback.

I built the entire tutoring system alone:

1. An **iPad app** (Swift) for handwriting input on linguistic puzzles.
2. A **NAO robot** (Qi Python) as the voice-user interface (VUI), letting participants discuss tasks with the robot in real time.
3. A **FastAPI backend** that organizes information and provides feedback.

## Contributions

- **Designed** the student-simulation pipeline, the data analysis, and the evaluation method, and wrote the first draft of the paper. We stress-tested the real-time multimodal system for robustness and used simulated students to examine the effectiveness of the tutor's feedback {% cite yueh2026adaptive %}.
- **Instantiated** prospect theory as an empathetic feedback algorithm for the robot tutor, deployed in a between-subjects learning experiment with human participants {% cite yueh2026empathic %}.
