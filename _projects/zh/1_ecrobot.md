---
layout: page
title: 智慧家教機器人 ECRobot
description: ECRobot（情感認知機器人）：具同理回饋設計的智慧教學系統
img: assets/img/ecrobot.png
importance: 1
category: lab
related_publications: true
lang: zh-TW
permalink: /zh/projects/1_ecrobot/
translation: /projects/1_ecrobot/
---

**[GitHub](https://github.com/hungchunchang/EmpathyCognitiveRobot)**

ECRobot（情感認知機器人）計畫旨在探討「同理心設計」對智慧教學系統（ITS）的影響，透過大型語言模型（LLM）生成具同理心的即時回饋，協助學生完成語言謎題。

本系統由本人獨立開發，歷時約三個月，包含三個主要模組：

1. **iPad 應用程式**（Swift 開發）：作為語言謎題的作答介面。
2. **語音使用者介面（VUI）**：讓參與者能與 NAO 機器人進行即時對話。
3. **FastAPI 後端**：負責資料庫管理並整合各模組。

同理心回饋演算法的設計基於**展望理論（Prospect Theory）**。

我們檢驗了這套即時多模態系統的效果與實用性：針對多模態輸入進行壓力測試以確保系統穩定，並以模擬學生檢驗系統回饋的效果。這項評估已發表於 *Enterprise Information Systems* {% cite yueh2026adaptive %}。
