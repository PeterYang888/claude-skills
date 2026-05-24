# Andrej Karpathy 決策模式與職涯選擇調研報告

**調研時間：** 2026-05-20

---

## 一、重大職涯決策

### 決策1：博士生 → OpenAI創始成員（2015）
- **當時選項：** 留學術界、加入業界（Google、DeepMind）、創業
- **選擇：** 加入OpenAI（非營利研究機構，創始團隊11人）
- **邏輯：** 使命（「推進AGI研究並使其對人類有益」）與他的核心關切高度吻合；機構研究是學術到工業的自然橋樑
- **他2015年在DeepMind深度強化學習組實習後，最終選擇OpenAI而非DeepMind**

### 決策2：OpenAI → Tesla AI總監（2017）
- **觸發：** Elon Musk主動招募（被形容為「全球電腦視覺領域第二強人，僅次於Ilya Sutskever」——法庭揭露的電子郵件）
- **吸引力：** 把電腦視覺真正部署在大規模現實系統（數百萬台車輛），而非純研究
- **決策邏輯：** 高風險但具備極高「現實驗證」價值——把學術研究直接落地的機會

### 決策3：Tesla離職 → 個人創作期（2022）
- **時間：** 2022年3月起休假，7月13日正式宣布離職
- **說法：** 「希望花更多時間重新投入對AI技術工作、開源與教育的長期熱情」
- **行動：** 立刻投入技術教學——Zero to Hero系列影片、nanoGPT等項目
- **信號：** 他在Tesla高管職位上長期渴望回到一線技術工作（「很期待有集中時間磨礪技術邊緣、訓練神經網路！」）

### 決策4：回歸OpenAI（2023/02）→ 再次離開（2024/02）
- **回歸邏輯：** ChatGPT成功後OpenAI熱度；組建中期訓練和合成資料新團隊
- **再次離開說法：** 「沒有任何事件或戲劇性情況」；想要「追求個人項目和獨立構建」

### 決策5：創立Eureka Labs（2024/07）→ 加入Anthropic（2026/05）
- **Eureka Labs核心使命：** 「融合我20年來對AI和教育熱情的結晶」；「讓全球任何人都能獲得頂尖AI教育」
- **選擇Anthropic而非回OpenAI：** 業界分析為「更看重前沿LLM的研究深度，而非組織歸屬感」
- **他的說法（加入Anthropic）：** 「LLM前沿的未來幾年將格外關鍵（especially formative）」

---

## 二、研究方向選擇邏輯

### 從電腦視覺到LLM的演化路徑（非突然轉變）

| 時間 | 方向 | 關鍵節點 |
|------|------|----------|
| 2011-2015 | 電腦視覺+語言交叉 | 博士論文：圖像與語言的細粒度對齊 |
| 2015 | 語言生成 | "Unreasonable Effectiveness of RNNs"——預見LLM時代 |
| 2017 | 軟體典範轉移 | Software 2.0：神經網路取代手寫程式碼 |
| 2022-2023 | LLM實作 | Zero to Hero系列，nanoGPT |
| 2023 | LLM宣言 | 「最熱門的程式語言是英文」 |
| 2026 | 前沿LLM研究 | 加入Anthropic預訓練團隊 |

### 「什麼研究值得做」的判斷標準

1. **可規模化（Scalable）**：一旦成立就能大規模運作的系統。這是他支持純視覺自動駕駛的核心理由，也是他對LLM著迷的原因
2. **可驗證（Verifiable）**：能夠用數據和結果驗證的路線，而非純理論爭論
3. **第一性原理（First Principles）**：「理解每一個細節才能做出偉大決策」
4. **有教育意義（Pedagogically Valuable）**：「做出來之後可以教給別人」——這個標準使研究和教學形成正向循環

---

## 三、Tesla Autopilot純視覺技術決策

### 核心論點（2021年CVPR演講）
- 「人類靠視覺開車——神經網路能夠從視覺輸入推斷深度和速度，答案毫無疑問是『能』」
- 「當雷達和視覺意見不同，你相信誰？視覺的精度遠高於雷達」
- LIDAR路線「需要預先建立高精地圖，這根本無法規模化到全地球」
- 組織論點：同時維護視覺堆疊和雷達堆疊，工程師注意力被稀釋；純視覺讓團隊集中在一條技術路線

### 業界爭議
- Waymo等公司堅持LIDAR+HD地圖路線，認為純視覺在惡劣天氣和邊緣案例有根本缺陷
- Tesla FSD在美國遭NHTSA調查（交通違規和事故報告）
- **Karpathy離職後的信號：** 他的警告「不要相信自動駕駛已經解決了」被部分人解讀為對過去路線的某種修正

### 此決策的決策邏輯特徵
- 在業界高度不確定的情況下，選擇了他認為「一旦成立就能無限泛化」的方案
- 願意接受短期的公眾批評，換取長期的技術路線一致性

---

## 四、教育投入的決策邏輯

### CS231n：為何在工業界仍繼續教學
他的核心邏輯：訓練下一代AI研究者是推進整個領域的槓桿行為，影響力遠超任何單一研究論文

### YouTube頻道的動機
- **青少年時期的原型：** 他曾在YouTube上有「badmephisto」頻道，教人解魔術方塊——顯示他從青少年時期就有「把複雜技巧拆解後教給別人」的本能
- **2022年爆發：** 離開Tesla後，精力回歸技術，Zero to Hero是第一個重大產出
- **他的教育哲學：** 「真正的學習不該是無摩擦的，應該感受到心智上的汗水（the mental equivalent of sweating）」

---

## 五、決策風格特徵

### 1. 高風險高回報傾向（每次職涯決策）
- OpenAI（未證明的新機構）→ Tesla（工業界高管）→ Eureka Labs（商業模式未成熟的教育創業）→ Anthropic（非OpenAI的選擇）
- 每次選擇都是「更難但更真實」的選項

### 2. 行動偏向（bias for action），前提是第一原理理解
- 他不等待不確定性消失，而是在理解透徹後快速押注
- Zero to Hero課程：不看現成框架，從空白Python文件建構GPT——「只有建構過才算真的懂」

### 3. 教育是「乘數器（Multiplier）」的核心信念
- 他相信最有影響力的事是「讓更多人能夠做好AI研究」
- 這是他一再回到教育的根本原因：單一研究論文的影響有限，但一套教材可以影響數萬名工程師

### 4. 數據勝過爭論
- 純視覺路線：不靠辯論，靠「1.5 PB的訓練數據和大規模部署」來驗證
- 教學方法：不靠說服，靠「讓學生自己從零建出來」來傳遞理解

### 5. 框架迭代，不固守舊說
- Software 2.0 → 3.0
- Vibe coding → Agentic engineering
- 他不會死守已發表的觀點，會公開更新框架

---

## 六、公開談到的人生哲學

### 對「什麼值得做」的判斷

**1. 追蹤「被低估的技術」**
他在2015年就在用RNN生成文字，那時這被認為是邊緣研究。他擅長提前看見哪些方向會爆發。

**2. 規模化是試金石**
他反覆用「scalable（可規模化）」作為判斷技術路線的最高標準——純視覺自動駕駛、LLM、Eureka Labs的教育模式，都是這個標準的體現。

**3. LLM是下一個計算典範**
> 他在2025年年度回顧中寫道：「LLM就像1970-80年代的個人電腦，我們目前只開發了其潛力的不到10%。」

**4. 對AI研究者的建議（A Survival Guide to a PhD，2016）**
- 博士的目標不是「發論文」，而是成為推動領域前進的社群成員
- 「要有勇氣有時候忽略你的導師，從第一性原理獨立思考」
- 「不要只玩既有的學術遊戲，要做別人沒有做但應該做的事」

---

## 主要來源
- http://karpathy.github.io/2016/09/07/phd/ （A Survival Guide to a PhD）
- https://karpathy.medium.com/software-2-0-a64152b37c35
- https://bdtechtalks.com/2021/06/28/tesla-computer-vision-autonomous-driving/ （純視覺立場）
- https://driveteslacanada.ca/news/andrej-karpathy-departs-tesla-sabbatical/
- https://techcrunch.com/2024/07/16/after-tesla-and-openai-andrej-karpathys-startup-aims-to-apply-ai-assistants-to-education/
- https://techcrunch.com/2026/05/19/openai-co-founder-andrej-karpathy-joins-anthropics-pre-training-team/
- https://karpathy.bearblog.dev/year-in-review-2025/ （2025年回顧）
- https://the-decoder.com/prominent-ai-researcher-andrej-karpathy-picks-anthropic-over-former-home-openai-to-get-back-into-frontier-llm-research/
