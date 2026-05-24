# Andrej Karpathy 著作與創作調研報告

**調研時間：** 2026-05-20
**來源規則：** karpathy.ai、karpathy.github.io、arxiv、GitHub、YouTube、可信技術媒體
**非政治人物，無需媒體偏向排除**

---

## 一、學術論文

### 最重要論文（按引用量排序）

| 排名 | 論文 | 年份 | 引用量 | 貢獻 |
|------|------|------|--------|------|
| 1 | ImageNet Large Scale Visual Recognition Challenge (ILSVRC) | 2015 | ~55,340 | 定義現代電腦視覺基準；合著者（第一作者為 Olga Russakovsky） |
| 2 | Large-scale Video Classification with ConvNets | 2014 CVPR | ~9,392 | 首次大規模將CNN應用於影片分類 |
| 3 | Deep Visual-Semantic Alignments for Generating Image Descriptions | 2015 CVPR | ~8,115 | **Karpathy 博士論文核心**；圖像區域與語言的細粒度對齊，第一作者 |
| 4 | Visualizing and Understanding Recurrent Networks | 2015 arXiv | ~1,614 | LSTM神經元可解釋性分析，發現個別神經元追蹤括號/URL等功能 |
| 5 | DenseCap: Fully Convolutional Localization Networks | 2016 CVPR | ~1,608 | 密集描述任務，對圖像每個局部區域生成文字，第一作者 |
| 6 | PixelCNN++: Improving the PixelCNN | 2017 ICLR | ~1,084 | 改進OpenAI生成模型；共同第一作者 |

**Google Scholar 總計：** 引用量 ~78,995，h-index: 11

**模式：** 第一作者主要是視覺-語言交叉研究（博士期間）；大型協作計畫（ImageNet、GPT-4o）為合著者

---

## 二、部落格文章（karpathy.github.io / karpathy.ai）

### 五篇最具代表性文章

**1. The Unreasonable Effectiveness of Recurrent Neural Networks（2015年5月）**
- 訓練字元級LSTM生成莎士比亞、LaTeX、Linux C、維基百科文字
- 核心論證：「序列模型是通用計算機」
- 解剖個別神經元，發現可解讀功能（追蹤引號狀態、行號等）
- **此文讓全球看見語言生成的潛力，是預見LLM時代的早期文獻**

**2. Software 2.0（2017年11月，Medium）**
- **最重要的思想文章**：提出神經網路是新的程式撰寫典範
- 核心命題：「資料集就是原始碼，梯度下降就是編譯器，模型權重就是二進位執行檔」
- 列舉視覺、語音、翻譯等領域中神經方法全面取代手工程式的案例
- 2025年進化為「Software 3.0」（LLM可用英文自然語言程式化）

**3. A Recipe for Training Neural Networks（2019年4月）**
- 實踐性六步訓練方法論，由Twitter串衍生
- 核心哲學：「神經網路訓練是帶滲漏的抽象層（leaky abstraction）」
- 關鍵步驟：徹底了解資料→建立簡單基線（過擬合單batch是必要步驟）→主動過擬合→正則化→調參→壓榨性能
- **至今仍是業界訓練神經網路的最佳實踐聖經**

**4. Deep Reinforcement Learning: Pong from Pixels（2016年5月）**
- 從Atari Pong原始像素出發，用130行Python實現Policy Gradient RL
- 教學風格典型：第一原理→最小程式碼→詳盡數學推導

**5. A Survival Guide to a PhD（2016年9月）**
- 博士生實用建議：選導師比選學校更重要、優先研究小型可複製子問題
- 「要成為某個非常特定領域的世界頂尖專家」
- 在AI研究社群廣泛流傳

**寫作風格特徵：**
- 技術深度高（含完整數學推導與可執行程式碼）
- 大量直覺性比喻（梯度 = 力、資料集 = 原始碼）
- 長篇深度（3,000-8,000字），結構清晰
- 第一人稱實驗紀錄（親身驗證每個主張）
- 更新頻率極低但每篇都有廣泛影響（2011-2026約19篇）

---

## 三、YouTube 教學影片（Andrej Karpathy 頻道）

### Neural Networks: Zero to Hero 系列（2022年8月起）

| # | 影片標題 | 核心內容 |
|---|---------|----------|
| 1 | The Spelled-Out Intro to NNs and Backprop: Building Micrograd | 從零建立autograd，手刻反向傳播 |
| 2-6 | Building Makemore (多集) | 字元級語言模型，從biagram到WaveNet |
| 7 | Let's Build GPT: From Scratch, in Code, Spelled Out | 完整實現GPT Transformer，attention機制 |
| 8 | Let's Build the GPT Tokenizer | 從零實現BPE tokenizer |

**獨立影片（重要）：**
- Intro to Large Language Models（2023，約1小時）：大眾版LLM解說
- Deep Dive into LLMs like ChatGPT（2025，約3.5小時）：技術深度版
- How I use LLMs（2025）：日常使用LLM工具展示

**教學哲學三原則：**
1. **從頭手刻（Build from scratch）**：一切從底層矩陣乘法和微積分開始
2. **最小程式碼（Minimal code）**：nanoGPT幾百行實現完整GPT
3. **第一原理（First principles）**：不接受「因為論文這樣說」的解釋

---

## 四、Twitter/X（@karpathy）

### 最常討論主題
- AI系統設計與資料策略（「按損失排序」是除錯資料最佳工具）
- GPT/Transformer架構
- Software 1.0 → 2.0 → 3.0的演化敘事
- 生物學與計算的類比（ATP合成酶、樹木是固化的空氣）
- 學習方法論
- 數位分心的危害（「通知的心理傷害是真實的」）

### 「Vibe Coding」原始推文
- **日期：** 2025年2月2日
- **原文（核心）：** "There's a new kind of coding I call 'vibe coding', where you fully give in to the vibes, embrace exponentials, and forget that the code even exists."
- **傳播：** 超過450萬次瀏覽；Collins英語詞典2025年度詞彙
- **Karpathy自評：** 「淋浴時的隨手一推」

### 代表性推文觀點
- 「梯度下降比人類更擅長寫程式碼。」
- 「資料的競爭優勢在於資料引擎——迭代式採集、重訓、評估、部署、遙測」
- 「通知對心理的傷害是真實的。」
- 「世界上最深度探索的節點在文明技術樹中，是半導體技術。」
- 「AGI是一種感覺，就像愛一樣。」

---

## 五、重複出現的核心信念（跨平台）

1. **第一原理至上：理解優先於使用** — micrograd、nanoGPT、microgpt均是「最小可理解實現」
2. **資料是AI系統的核心資產** — 「真正的競爭優勢在於迭代式資料採集與評估循環」
3. **最小且完整的程式碼是最好的教學工具** — 「程式碼複雜度是理解的最大障礙」
4. **AI正在重寫軟體工程範式（1.0→2.0→3.0）** — 他是這一敘事最早且最一貫的倡導者
5. **AI教育是當代最重要使命之一** — CS231n→Zero to Hero→Eureka Labs一脈相承
6. **快速迭代是AI研究的核心競爭力** — autoresearch（兩天內自主700次實驗）
7. **生物學是計算的終極參照系** — 對ATP合成酶、神經架構、進化演算法的深度著迷

---

## 最新動態（截至2026年5月）

**2026年5月19日**：宣布加入Anthropic預訓練團隊（Nick Joseph帶領下），主導「以Claude加速預訓練研究」的新方向。

---

## 主要來源
- https://karpathy.ai / https://karpathy.github.io
- https://karpathy.medium.com/software-2-0-a64152b37c35
- https://karpathy.ai/zero-to-hero.html
- https://x.com/karpathy/status/1886192184808149383 (vibe coding)
- https://x.com/karpathy/status/1617979122625712128 (hottest programming language)
- https://scholar.google.com/citations?user=l8WuQJgAAAAJ
- https://techcrunch.com/2026/05/19/openai-co-founder-andrej-karpathy-joins-anthropics-pre-training-team/
