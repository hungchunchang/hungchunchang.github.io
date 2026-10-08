---
layout: page
title: 高齡陪伴機器人
description: 高齡陪伴對話機器人的設計探索
img: assets/img/robocom.jpg
importance: 3
related_publications: true
category: lab
lang: zh-TW
permalink: /zh/projects/3_robots_for_elderly/
translation: /projects/3_robots_for_elderly/
---

**[專案網站](https://socrobot.ntu.edu.tw/Robert's%20House/index.html#)**
**[GitHub](https://github.com/Jason0102/xiaoxiao_v1)**

這是一系列為高齡者設計、提供持續互動的社會機器人，目的是透過對話代理人促進**自我揭露（self-disclosure）**行為。機器人的角色設定為一位剛畢業的大學生，藉由分享自身的生活經驗，以自然對話引導使用者分享個人經驗與想法。

## 曉曉

**資料分析與前端開發** · 2024 年 3 月 – 2025 年 12 月  
_International Journal of Human–Computer Interaction_, 2026

曉曉（XiaoXiao）是一款專為高齡使用者設計的陪伴型機器人，具備融入背景故事情境的**語音使用者介面（VUI）**，引導使用者進行自然且深入的對話。初步的設計構想與使用者測試結果發表於 **ARIS 2024** {% cite lo2024memory %}。

主要特色：

- 背景故事框架，為對話提供情境脈絡
- 語音介面，不依賴圖形介面流暢互動
- 以高齡科技（gerontechnology）為基礎的使用者中心設計

在比較高情感與低情感機器人個性的實驗中 {% cite yueh2026makes %}，我：

- **開發前端介面**，在對話中呈現機器人的回應。
- **為操弄檢核以語意定義機器人刺激**——把對話的情感性操作化為可量測的語言指標，並據此驗證兩台機器人的對話內容確實如設計般不同。

每次對話平均 **15 分鐘**，每位參與者平均 **30 分鐘**。

## 學士論文：日記機器人 Zbot {#bachelors-thesis}

_基於社會滲透理論之高齡對話機器人設計與評估_（Design and Evaluation of a Conversational Robot for the Elderly Based on Social Penetration Theory）

學士論文中，我開發了高齡日記機器人 Zbot：沿用曉曉的前端，並開發新的後端。機器人以社會滲透理論為基礎，設計成在對話過程中引導高齡者逐步揭露更多關於自己的事。本研究共進行 **28 次使用者研究、與 7 位高齡者互動，歷經 4 次系統迭代**。

**從行為而非問卷測量自我揭露。** 傳統的自我揭露量表題目冗長、無法捕捉即時行為，也可能有不誠實作答的問題。我建立了自我揭露的行為構念，以及直接從對話中量測它的多模態分析架構，發表於 **DADH 2025** {% cite chang2025assessment %}：

- **語言層面：** 以 LIWC 字典分析參與者話語中的情緒、認知與社會歷程特徵。
- **語音層面：** 以傳播適應理論（Communication Accommodation Theory）為架構，用語音*同步*（對話雙方彼此趨近的程度）作為人際態度指標——以 Praat 分析音高（F0）與音色（harmonicity），以 Librosa 擷取 MFCC 與 LTAS 等頻譜特徵。

開發 Zbot 的經驗也是[社會機器人設計平台](/zh/projects/4_desiging_social_robots/)背後的系統之一。
