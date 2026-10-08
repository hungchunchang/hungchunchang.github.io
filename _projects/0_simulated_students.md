---
layout: page
title: Validity of LLMs as Simulated Students
description: Master's thesis — can an ability-conditioned LLM stand in for real learners?
img:
importance: 1
category: lab
related_publications: true
translation: /zh/projects/0_simulated_students/
---

**Master's thesis (in progress)** · Feb. 2026 – present  
Advisors: Prof. Hsiu-Ping Yueh, Prof. Feng-Ming Tsao, and Prof. Hiroaki Ogata (Kyoto University)

LLM-based "simulated students" are increasingly used to test tutoring systems and generate learner data, usually by telling a model to act like a student of a given ability. Whether such a simulator actually behaves like students of that ability is rarely tested as a construct. My thesis asks that question directly.

- **Recast** the validity of an ability-conditioned LLM student simulator as a nomological network of four behavioral evidences: profile–behavior consistency, fidelity of error, boundary of competence, and stateful learning.
- **Tested** all four concurrently against real per-tier learner data from the PSLC DataShop Fractions 2012 corpus, using zero-shot prompting and a 2 × 2 fine-tuning ablation (reasoning × history).
- **Found** that fine-tuning with reasoning and history simulated students best, yet the competence paradox persisted and the learning mechanism was not reproduced.

The first part of this work was carried out as an international collaboration during my research internship at Kyoto University and accepted at the ReLEAF workshop at ICCE 2026 {% cite chang2026does %}.
