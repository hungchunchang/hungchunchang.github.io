---
layout: page
title: 以 LLM 作為模擬學生的效度
description: 碩士論文——依能力設定的 LLM 能否代替真實學習者？
img:
importance: 1
category: lab
related_publications: true
lang: zh-TW
permalink: /zh/projects/0_simulated_students/
translation: /projects/0_simulated_students/
---

**碩士論文（進行中）** · 2026 年 2 月至今  
指導教授：岳修平教授、曹峰銘教授、緒方広明教授（京都大學）

以 LLM 打造的「模擬學生」越來越常被用來測試教學系統、產生學習者資料，做法通常是要求模型扮演某個能力程度的學生。但這樣的模擬器是否真的表現得像那個能力程度的學生，很少被當成一個構念來檢驗。我的碩士論文正面處理這個問題。

- **重構**：把依能力設定的 LLM 模擬學生之效度，重新界定為由四種行為證據組成的法則網絡（nomological network）：能力設定與行為的一致性、錯誤的擬真度、能力邊界，以及具狀態的學習。
- **檢驗**：以 PSLC DataShop Fractions 2012 語料中各能力層級的真實學習者資料，同時檢驗這四項證據；比較零樣本提示，以及 2 × 2 的微調消融設計（推理 × 歷程）。
- **發現**：同時以推理與歷程微調的模型最能模擬學生，但「能力悖論」依然存在，學習機制也未被重現。

第一部分的研究在京都大學研究實習期間以國際合作方式完成，已被 ICCE 2026 的 ReLEAF 工作坊接受 {% cite chang2026does %}。
