---
layout: post
title: 2026九月對於最近AI發展的想法
date: 2025-09-30 15:30:16
description: recent thoughts on using ai in sep 2025
tags: genai personal
categories: on_ai
published: true
---

## Recent Development of AI&LLM

殘酷而現實的說，目前為止以 transformer 為基礎的大模型，幾乎打敗了過去幾十年人工智慧在各個領域上的進展，彷彿一切只要套用大模型，所有問題就能迎刃而解。

然而，在實際部署上，大多數基於大模型 AI 在實際應用上，都以失敗告終。歸根究底，就是大語言模型充其量，只能是 SaaS 中重要且不可或缺的一環，「在系統都不能學習、讀不懂情境（context）、也沒辦法越用越好用的情況下，無法真正接手組織的核心流程。」（Dr. Harvey的某一篇電子報）。

此外，由於 AI 能夠生成「還不錯」的程式碼，對於沒有軟體工程師的團隊而言，能夠快速產出原型，但接下來才是棘手的部分：修正 AI 的錯誤、對原型進行迭代等。因為缺乏維護知識，既無法有效率的修改 AI 的錯誤，也無法進行迭代，結果就是團隊有且僅有原型，而沒辦法真正產出可用的產品。

### Context Engineering

雖然情境工程聽起來像是下一個提示詞工程、檢索增強生成，在人工智慧浪潮的風口浪尖上製造話題，在誠品擺滿一整櫃的教學書。但至少就我的觀點看來，情境工程別具意義。

首先，情境工程的出現，用意是彌補提示詞工程、檢索增強生成等不同大語言模型應用技巧的不足，回應。報告（Maslej, 2025）中，明確表明 AI 應用無法落地生根的窘境。

研究契機：可以調查使用者對於 AI 的認知、期望，並且分析實際上使用的落差，我認為代理人感（sense of agency）是一個良好的切入點，因為 LLM 展現出如人一樣的回應能力，以及看似存在的推理能力。然而，LLM 的推論並不符合人類的直觀（intuition），而是服從統計規律性，加上訓練過程中，在訓練規則的鼓勵下出現幻覺 Kalai et al. (2025)，因此大語言模型完全稱不上可靠。

情境工程的內涵可以主要分為三者：

1. 指導性上下文（Guiding Context）：設定模型行為的框架、目標和規則，包括系統提示詞（system prompt）、任務描述、少樣本範例（few-shot examples）和輸出格式定義。
2. 資訊性上下文（Informational Context）：為模型提供解決問題所需的事實、數據與知識，包括檢索增強生成（RAG）、短期記憶（如 scratchpad）和長期記憶。
3. 行動性上下文（Actionable Context）：提供模型與外部世界互動的能力，包括工具定義、工具調用及其結果，以及工具追蹤。

上下文工程的目標是確保 AI 回覆更穩定、減少錯誤和意外。它的關鍵操作包括寫入（writing）、選取（selecting）、壓縮（compressing）和隔離（isolating）。許多 AI Agent 的失敗並非模型能力不足，而是上下文工程的失敗。

因此，情境工程或許可以成為大語言模型實現落地應用的關鍵之一。從使用者研究的角度而言，缺乏對使用情境的理解，便難以設計出真正好用的系統；對於社會機器人研究來說，具有自然語言互動的能力，

在人機互動、社會機器人的研究中，早已出現類似於情境工程的研究方法 (Syrdal et al., 2014; Koay et al., 2020; Leite et al., 2017)。

Koay et al. (2020) 期望設計出具有沈浸感的原型，也衍伸出下列規則：

- 互動規則：
  - 必須基於真實的科技發展
  - 必須在情境中自然發生
  - 必須在連續時間內發生
- 參與者規則
  - 必須將環境視為自身所處
  - 必須盡力與機器人互動達到目標
  - 能夠將科技與他的行為擬人化
- 技術應該
  - 基於對系統發展的現實預測。
  - 影響其所處的敘事

### 缺口與動機

綜合而言，現有的大模型能夠在特定任務上達成傑出的表現，然而，人類生活中的情境多元，環境複雜，因此現有的大模型無法任意的安插在特定工作崗位，作為即時的生力軍。想要解決此一問題，就只要提升模型的適應能力，除了在訓練時，就為模型設計合理的學習能力，符合使用情境的需求探索也很重要，透過理解真實的使用情境，為模型提供情境資訊（context），包含指導性情境資訊、資訊性情境資訊、行動性情境資訊，也能增加模型的適應能力。此外，透過情境設計，也能降低非程式設計專業人員的維護成本，使得長期維持 AI 應用可能性大幅提升。

## Reference


- Kalai, A. T., Nachum, O., Vempala, S. S., & Zhang, E. (2025). Why language models hallucinate. arXiv preprint arXiv:2509.04664.
- Koay, K. L., Syrdal, D. S., Dautenhahn, K., & Walters, M. L. (2020). A narrative approach to human-robot interaction prototyping for companion robots. Paladyn, Journal of Behavioral Robotics, 11(1), 66-85.
- Leite, I., McCoy, M., Lohani, M., Ullman, D., Salomons, N., Stokes, C., ... & Scassellati, B. (2017). Narratives with robots: The impact of interaction context and individual differences on story recall and emotional understanding. Frontiers in Robotics and AI, 4, 29.
- Maslej, N. (2025). Artificial Intelligence Index Report 2025. Artificial Intelligence.
- Syrdal, D. S., Dautenhahn, K., Koay, K. L., & Ho, W. C. (2014). Views from Within a Narrative: Evaluating Long-Term Human-Robot Interaction in a Naturalistic Environment Using Open-Ended Scenarios. In Cognit Comput (Vol. 6, Issue 4, pp. 741–759). https://doi.org/10.1007/s12559-014-9284-x
- 最佳拍檔. (2025, August 14). 【人工智能】什么是上下文工程Context Engineering \| 上下文Context \| Agent的缺点 \| 提示词工程 \| RAG \| MCP \| 写入 \| 选取 \| 压缩 \| 隔离 [Video recording]. https://www.youtube.com/watch?v=0J20wMjfuEc
- 最佳拍檔. (2025, August 14). 【人工智能】什么是上下文工程Context Engineering \| 上下文Context \| Agent的缺点 \| 提示词工程 \| RAG \| MCP \| 写入 \| 选取 \| 压缩 \| 隔离 [Video recording]. https://www.youtube.com/watch?v=0J20wMjfuEc

