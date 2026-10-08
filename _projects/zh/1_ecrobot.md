---
layout: page
title: 智慧家教機器人 ECRobot
description: ECRobot（情感認知機器人）：具同理回饋設計的智慧教學系統
img: assets/img/ecrobot.png
importance: 2
category: lab
related_publications: true
lang: zh-TW
permalink: /zh/projects/1_ecrobot/
translation: /projects/1_ecrobot/
---

**[GitHub](https://github.com/hungchunchang/EmpathyCognitiveRobot)**

**獨立開發** · 2025 年 9 月 – 2025 年 12 月  
*Enterprise Information Systems*, 2026；*Educational Psychology*，修改中

ECRobot（情感認知機器人）計畫旨在探討「同理心設計」對智慧教學系統（ITS）的影響，透過大型語言模型（LLM）生成具同理心的即時回饋，協助學生完成語言謎題。

整套教學系統由我獨立開發：

1. **iPad 應用程式**（Swift）：語言謎題的手寫作答介面。
2. **NAO 機器人**（Qi Python）：作為語音使用者介面（VUI），讓參與者能與機器人即時討論題目。
3. **FastAPI 後端**：整理資訊並提供回饋。

## 我的貢獻

- **設計**模擬學生流程、資料分析與評估方法，並撰寫論文初稿。我們對這套即時多模態系統進行壓力測試以確保穩定，並以模擬學生檢驗系統回饋的效果 {% cite yueh2026adaptive %}。
- **將展望理論（prospect theory）實作**為機器人家教的同理回饋演算法，並用於以真人參與者進行的受試者間學習實驗 {% cite yueh2026empathic %}。
