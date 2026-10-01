---
layout: page
title: ECRobot
description: ECRobot (Empathy Cognition Robot) — an Intelligent Tutoring System with empathetic feedback design
img: assets/img/ecrobot.png
importance: 1
category: lab
related_publications: true
translation: /zh/projects/1_ecrobot/
---

**[GitHub](https://github.com/hungchunchang/EmpathyCognitiveRobot)**

The ECRobot (Empathy Cognition Robot) project investigates the effect of empathetic design on intelligent tutoring systems (ITS). The system assists students in completing linguistic puzzles with LLM-generated, empathetic real-time feedback.

Developed individually over 3 months, the system consists of three main components:

1. A customized **iPad app** (Swift) as the answering interface for linguistic puzzles.
2. An **interactive voice-user interface (VUI)** allowing participants to discuss tasks with the NAO robot in real time.
3. A **FastAPI backend** handling database management and connecting all components.

The empathetic feedback algorithm is grounded in **Prospect Theory**.

We examined the effectiveness and utility of the intelligent tutoring system ECRobot, a realtime multimodal system. For system robustness, we implemented stress tests towards multimodal inputs. On top of that, we utilized simulated students for examining the effectiveness of feedback from the ITS. This evaluation was published in *Enterprise Information Systems* {% cite yueh2026adaptive %}.
