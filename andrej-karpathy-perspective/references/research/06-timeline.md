# Andrej Karpathy 生平時間軸調研報告

**調研時間：** 2026-05-20

---

## 一、生平基本資料

| 項目 | 資料 | 可信度 |
|------|------|--------|
| 出生日期 | 1986年10月23日 | ✅ 高（多媒體確認） |
| 出生地 | 布拉提斯拉瓦（Bratislava） | ✅ 高 |
| 出生時國籍 | 捷克斯洛伐克（政治名義），但地理上是斯洛伐克 | ✅ 高（需澄清） |
| 現國籍 | 斯洛伐克裔加拿大人（Slovak-Canadian） | ✅ 高（他本人自稱） |
| 移民時間 | 約2001年（15歲時）移居加拿大多倫多 | ✅ 高 |

**常見誤記：** 說他「出生於捷克」或「捷克裔」——他是斯洛伐克裔。1986年出生時布拉提斯拉瓦法律上屬捷克斯洛伐克，但地理上一直是斯洛伐克的首都（1993年正式獨立後成為首都）。

---

## 二、學歷時間軸

| 時間 | 機構 | 學位 | 備注 |
|------|------|------|------|
| 2005-2009 | 多倫多大學（University of Toronto） | 電腦科學與物理學士 | — |
| 2009-2011 | 英屬哥倫比亞大學（UBC） | 電腦科學碩士 | 導師：Michiel van de Panne；論文方向：物理模擬角色的控制器學習 |
| 2011-2015 | 史丹佛大學（Stanford University） | 電腦科學博士 | **導師：李飛飛（Fei-Fei Li）**；研究方向：深度學習、電腦視覺 |

---

## 三、精確職涯時間軸

| 時間 | 事件 | 重要性 |
|------|------|--------|
| 2015年（夏） | 在DeepMind深度強化學習組實習 | 接觸RL；最終選擇OpenAI而非DeepMind |
| 2015/12 | 加入OpenAI（創始成員） | 11位創始成員之一；職稱：研究科學家 |
| 2015 | 設計並主講Stanford CS231n（深度學習課程） | 全球影響最廣的深度學習公開課之一 |
| 2017/06 | 加入Tesla，職稱AI及Autopilot Vision總監 | 直接向Elon Musk匯報 |
| 2021/06 | CVPR演講，為純視覺自動駕駛路線辯護 | Tesla技術路線的最重要公開聲明 |
| 2022/03 | 開始四個月薩巴提卡（sabbatical） | 休假期間開始技術寫作 |
| **2022/07/13** | **正式離開Tesla** | ⚠️ 常見誤記為2023年，實為2022年 |
| 2022/08 | 開始YouTube系列「Neural Networks: Zero to Hero」 | 首集：Building Micrograd |
| 2022/12 | nanoGPT首次提交GitHub | 精簡GPT實現 |
| 2023/01/24 | 發推「The hottest new programming language is English」 | LLM時代宣言 |
| 2023/02/09 | 重返OpenAI（第二次） | 組建中期訓練和合成資料新團隊 |
| 2024/02/13 | 再次離開OpenAI（第二次離職） | 「沒有任何事件或戲劇性情況」 |
| 2024/07/16 | 創立Eureka Labs，宣布LLM101n課程 | AI原生教育公司 |
| 2025/02/02 | 發推「vibe coding」 | Collins 2025年度詞彙；450萬+次瀏覽 |
| 2025/06 | YC AI Startup School演講「Software Is Changing (Again)」 | Software 3.0完整論述 |
| 2026/02/12 | 推出microGPT（200行純Python實現GPT） | 最小化教學項目 |
| **2026/05/19** | **加入Anthropic預訓練團隊** | 最新動態 |

---

## 四、主要開源項目時間軸

| 項目 | 時間 | 目的 | GitHub Stars |
|------|------|------|-------------|
| micrograd | 2020 | 教學：標量autograd引擎（~150行） | 15,900+ |
| nanoGPT | 2022/12 | 教學+實用：最簡GPT預訓練實現 | 58,500+ |
| llm.c | 2024（上半年） | 教學+研究：用~1000行C/CUDA實現GPT-2訓練 | — |
| microGPT | 2026/02/12 | 教學：200行純Python、零依賴GPT | — |

---

## 五、CS231n課程歷史

- **首次開課：** 2015年冬季學期（與李飛飛、Justin Johnson共同設計）
- **全名演化：** CS231n: Convolutional Neural Networks for Visual Recognition → CS231n: Deep Learning for Computer Vision
- **招生成長：** 2015年150人 → 2016年330人 → 2017年750人
- **YouTube觀看：** 累計超過80萬次
- **目前狀態：** Karpathy離開Stanford後已不再主講；課程仍在Stanford持續開設（⚠️ 目前具體授課教師待確認）

---

## 六、常見誤記整理

| 誤記 | 正確資訊 |
|------|---------|
| 「捷克裔」或「出生於捷克」 | 斯洛伐克裔；布拉提斯拉瓦在地理上是斯洛伐克 |
| 離開Tesla說成「2023年」 | **實際為2022年7月13日** |
| 稱他為OpenAI「聯合創始人（co-founder）」 | 更精確說法是「創始成員（founding member）」；他是研究科學家，非管理層主要創辦人 |
| Eureka Labs「只是計畫」或「尚未成立」 | **已正式成立並發布產品（LLM101n）**，Crunchbase有記錄 |
| 認為他至今仍在Eureka Labs | 2026年5月已加入Anthropic |

---

## 七、個人背景對思維的影響

- **15歲移民加拿大**：這段「後來者」經歷使他對教育平等與知識普及有深刻體會
- **他在Eureka Labs的使命**：「讓全球任何人都能獲得頂尖AI教育」——移民背景的直接投射
- **開源項目設計哲學**：刻意保持代碼極簡，體現「讓知識可觸及」的信念
- **青少年時期YouTube（badmephisto頻道）**：教魔術方塊解法——「把複雜技巧拆解後教給別人」的本能從那時就已存在
- 公開談論個人成長經歷的訪談：**待確認**（Lex Fridman等訪談中有相關片段，具體內容需進一步核實）

---

## 主要來源
- https://en.wikipedia.org/wiki/Andrej_Karpathy
- https://cs.stanford.edu/people/karpathy/
- https://cs.stanford.edu/~karpathy/Andrej_Karpathy_Resume.pdf
- https://www.cnbc.com/2022/07/13/tesla-ai-leader-andrej-karpathy-announces-hes-leaving-the-company.html （Tesla離職，2022/07）
- https://techcrunch.com/2024/02/13/andrej-karpathy-is-leaving-openai-again-but-he-says-there-was-no-drama/
- https://www.maginative.com/article/andrej-karpathy-launches-eureka-labs-an-ai-native-school/
- https://techcrunch.com/2026/05/19/openai-co-founder-andrej-karpathy-joins-anthropics-pre-training-team/
- https://www.bloomberg.com/news/articles/2026-05-19/openai-founding-member-andrej-karpathy-takes-role-at-anthropic
- https://github.com/karpathy/nanoGPT
- https://github.com/karpathy/micrograd
