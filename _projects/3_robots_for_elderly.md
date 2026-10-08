---
layout: page
title: Companion Robot (Xiao Xiao)
description: An exploration on designing conversation social robot
img: assets/img/robocom.jpg
importance: 3
related_publications: true
category: course
translation: /zh/projects/3_robots_for_elderly/
---

**[Project Website](https://socrobot.ntu.edu.tw/Robert's%20House/index.html#)**
**[GitHub](https://github.com/Jason0102/xiaoxiao_v1)**

RoboCom is a social robot designed to provide sustained interaction with older adults. The core goal is to induce **self-disclosure** through a carefully designed conversation agent — a persona of a recently graduated college student who shares stories from their own life to invite the user to share theirs.

Our first product is XiaoXiao, a companion robot for older adults featuring a **voice-user interface (VUI)** with background storytelling to encourage extended, natural conversation. Primary design and user testing results were presented at **ARIS 2024** {% cite lo2024memory %}.

Key features:

- Background narrative framing to provide conversation context
- VUI enabling fluid spoken interaction without screen dependency
- Iterative user-centered design grounded in gerontechnology

## My contributions

**Bachelor's thesis.** The project served as the foundation of my bachelor's thesis, involving **28 user research sessions with 7 older adults across 4 system iterations**.

**Measuring self-disclosure from behavior, not questionnaires.** Self-report scales of self-disclosure are long, cannot capture behavior as it happens, and are open to dishonest answers. I built a behavioral construct of self-disclosure and a multimodal pipeline to measure it from the conversations themselves, presented at **DADH 2025** {% cite chang2025assessment %}:

- **Language:** LIWC dictionaries to code emotional, cognitive, and social-process markers in what participants said.
- **Speech:** grounded in Communication Accommodation Theory, vocal *entrainment* (how speakers converge toward each other) as an index of interpersonal attitude — pitch (F0) and harmonicity with Praat, and spectral features (MFCC, LTAS) with Librosa.

**Affective robot personalities (IJHCI 2026).** For the follow-up experiment comparing a high-affective and a low-affective robot {% cite yueh2026makes %}, I:

- **Developed the front-end app** that presents the robot's responses during conversation.
- **Defined the robot stimuli semantically for the manipulation check** — operationalizing discourse affectiveness into measurable linguistic indicators, and using them to verify that the two robots' conversational turns actually differed as designed.

Conversations averaged **15 minutes** per session and **30 minutes** per participant.
