# Andrej Karpathy 表達DNA與語言風格調研報告

**調研時間：** 2026-05-20

---

## 一、他自創或普及的術語

| 術語 | 出處 | 時間 | 可信度 |
|------|------|------|--------|
| **Software 2.0** | Medium文章 | 2017年 | ✅ 高（他原創） |
| **The hottest new programming language is English** | X推文 | 2023/01/24 | ✅ 高（原始推文可查）|
| **Software 3.0** | YC AI Startup School演講 | 2025年6月 | ✅ 高 |
| **Vibe coding** | X推文（2025/02/02） | 2025年2月 | ✅ 高（有原始推文）|
| **Context engineering**（普及） | X推文 | 2025年6月 | ✅ 中（他普及，非原創） |
| **People spirits**（LLM比喻） | Software 3.0演講 | 2025年 | ✅ 高 |
| **Jagged intelligence** | Deep Dive into LLMs影片 | 2025年 | ✅ 高（注：jagged frontier原出自Ethan Mollick，他使用變體） |
| **Anterograde amnesia**（LLM比喻） | X推文與演講 | 2025年 | ✅ 高 |
| **Autonomy slider** | Software 3.0演講 | 2025年 | ✅ 高 |
| **Agentic engineering** | No Priors Podcast | 2026年 | ✅ 高 |

**注意：** 「Software is eating the world, but AI is eating software」這句話**不是Karpathy說的**，原版出自Marc Andreessen（2011）。Karpathy的說法更接近「Software 3.0 is eating 1.0/2.0」。

---

## 二、類比使用模式（最具識別度的語言特徵）

### 物理與機械類比（解釋梯度與反向傳播）
- 梯度 = **「力（force）」或「拉力（tug）」**：「把梯度想像成一個力，拉著輸入往某個方向走」
- 反向傳播 = 電路中的力傳遞（從末端施加拉力，分配回整個電路）
- 正則化 = **彈簧的Hooke's law**（將參數拉向零的力）
- Max gate = 梯度的**實體路由器**

### 神經病理學隱喻（LLM的限制）
- LLM無持續學習 = **順行性失憶症（anterograde amnesia）**：「就像得了順行性失憶症的同事」
- LLM能力不均 = **Jagged intelligence**

### 人格化/心理學隱喻（LLM的本質）
- LLM = **「人類靈魂的隨機模擬（stochastic simulations of people）」**，也稱 "people spirits"
- 電影類比（Software 3.0演講）：Rain Man（天才但受限）、Memento（失憶）、50 First Dates（每次重置）

### 作業系統類比（LLM生態）
- LLM = CPU；context window = RAM；weights = 長期記憶
- 整個LLM生態 = 新型OS，closed-source（OpenAI/Anthropic）vs open-source（Llama）= Windows vs Linux

### 資料類比（Software 2.0）
- Dataset = 程式的「源碼」；訓練 = 編譯

---

## 三、「Software 2.0」思維框架

**2017年Medium文章核心命題：**
> 「In Software 2.0, the dataset is the source code.」

**三個範式的完整演化：**
- **Software 1.0**：人類撰寫明確指令（Python、C++等）
- **Software 2.0**：人類策劃資料集，神經網路自己「寫出」函數
- **Software 3.0**（2025年）：LLM是可以用自然語言（英文）程式化的新型電腦，prompts = programs

**此框架代表他思維的特徵：**
1. 範式轉移思維（談根本性典範替換，不談優化）
2. 工程師視角的哲學（把「程式設計是什麼」轉化為可操作框架）
3. 預言性格局（2017年就預言軟體工程師角色將重新分工）

---

## 四、教學語言特徵

### 課程標題的品牌語言
- **「Spelled-out」**（詳細闡明，一步步拆解）
- **「From scratch」**（從零開始）
- **「In code」**（在程式碼中實現）
- **「Let's build」**（邀請觀眾一起做，而非示範）

代表標題：「The **Spelled-Out** Intro to Neural Networks: **Building** Micrograd **From Scratch**」

### 課堂口語模式
- **"Let me show you..."**（示範導向）
- **"And by the way..."**（補充說明，保持口語流）
- **"This is actually really simple..."**（反直覺的簡化，降低焦慮感）
- **"Let me just verify this numerically..."**（數值驗證習慣）
- **"I want to build an intuition for..."**（明確宣告目標是直覺，不是死記）
- **"Don't be a hero"**（提醒學生不要過早引入複雜性）

### 從直覺到數學的固定路徑
1. **直覺先行**：用物理比喻或視覺化建立感受
2. **程式碼實作**：在Python/NumPy把直覺變成可執行的東西
3. **數學驗證（非核心）**：數學公式是最後才出現的確認工具，不是入口

**他的哲學：** 「95%的backpropagation材料都在以錯誤的方式呈現它」——先讓你理解發生了什麼，再告訴你符號怎麼寫。

---

## 五、Twitter語言風格

### 推文長度偏好：雙峰分布
- **短而有力的格言式推文**（一句話）：「The hottest new programming language is English.」（11個詞）
- **中等長度說明型推文**：多句話解釋技術概念，通常附連結

**Karpathy自評：** vibe coding那則推文是「shower of thoughts throwaway tweet I just fired off」——說明短推文往往是即興的

### 表情符號使用
- **極少使用**，偶爾策略性使用🤔（表示推測）
- 整體風格：表情符號是強調工具，不是裝飾

### 內容分佈：觀點推文略多於技術推文（約6：4）

---

## 六、英文寫作風格特徵

### 句子長度：短長交替節奏
- 短句製造衝擊：「They work better in practice.」「Don't be a hero.」「This is insane.」
- 長句建立論證，通常4行內插入短句重置節奏

### 語態：強烈偏好主動語態（個人化、直接）

### 標點符號習慣
- **大量使用破折號（em dash）**：插入補充說明，代替括號
- **常用冒號（:）**：引導解釋性說明
- **引號標記新概念**：先包住術語再正式定義
- **括號作為旁白**：個人反思、承認局限、自我調侃

### 整體語氣
- 坦誠度高（「我試過，很難」「這有點難看」）
- 包容性 "we"：把讀者拉進來，而非俯視式說教
- 強調詞癖："really"「reeaally」（故意拼錯強調）「for sure」「quite」
- 樂觀但輕描淡寫：「quite astonishing」「really quite great」——保持可信度

---

## 七、知名語錄核實

### ✅ 「The hottest new programming language is English」
- **確認是Karpathy原創**
- 日期：2023年1月24日
- 來源：https://x.com/karpathy/status/1617979122625712128

### ✅ 「Vibe coding」原始推文
- 日期：2025年2月2日
- 來源：https://x.com/karpathy/status/1886192184808149383
- 核心：「There's a new kind of coding I call 'vibe coding', where you fully give in to the vibes...」
- Collins Dictionary 2025年度詞彙

### ❌ 「Software is eating the world, but AI is eating software」
- **這句話不是Karpathy說的** — Marc Andreessen原版（2011）的延伸；此引句的Karpathy版本不可信，不應直接歸因

---

## 八、語言DNA特徵總結

| 維度 | 特徵 |
|------|------|
| **框架思維** | 總在建構大敘事（1.0/2.0/3.0），拒絕孤立討論技術細節 |
| **類比策略** | 物理力學→神經病理學→電影/流行文化，越來越人性化 |
| **教學哲學** | 直覺優先，程式碼為橋梁，數學為確認，「from scratch」為原則 |
| **語氣矛盾** | 專家的精確+朋友的隨意；驚嘆的低調+批評的坦率 |
| **術語立場** | 精確定義自己的詞（避免濫用"AI"、"GPT"），創造新詞填補空缺 |
| **推特基因** | 短句格言+即興洞見，表情符號稀少，觀點與技術各半 |
| **版本管理** | 概念會迭代升級（vibe coding → agentic engineering），不固守舊說 |
