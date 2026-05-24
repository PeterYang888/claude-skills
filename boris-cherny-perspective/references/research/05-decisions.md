# Boris Cherny 決策模式與職涯選擇調研報告

**調研時間：** 2026-05-20

---

## 一、重大職涯決策

### 決策1：早期新創 → Meta（2017）
- **背景：** 在多個早期新創工作後，加入 Meta（當時為 Facebook）
- **角色：** 前端工程師（IC4），後晉升至 IC8（7年間）
- **邏輯：** Meta 是全球規模最大的前端工程生態之一；在那裡能接觸到真正的規模挑戰
- **主要貢獻：**
  - 開發 json-schema-to-typescript（解決大規模前端工程的類型定義問題）
  - 開發 undux（輕量狀態管理）
  - 深度使用 Flow（TypeScript 的競爭對手）
  - 撰寫《Programming TypeScript》（利用業餘時間，2019年出版）

### 決策2：Meta → Anthropic（2024年9月）
- **觸發：** AI 編程工具機會；看到「latent demand」——工程師在用 GitHub Copilot 等工具但沒有真正整合的工作流
- **吸引力：** 從零建構一個新類別的產品；Claude 的代碼能力足夠強大
- **決策邏輯：** 「工程師已經在用 AI 工具了，但他們在用錯誤的工具。沒有人給他們一個真正在終端機工作的 AI。」
- **結果：** 創建 Claude Code，從 0 到成為主流 AI 編程工具之一

### 決策3：Anthropic → Cursor（2025年7月，短暫）
- **時間：** 2025年7月
- **觸發：** Cursor 積極招募；對「做更自主的 AI IDE」的興趣？（具體原因未公開）
- **職位：** Chief Architect（首席架構師）
- **時長：** ~2週
- **返回 Anthropic 的原因：** 未公開說明；業界推測是意識到 Claude Code 的影響力更大，或文化/使命感問題

### 決策4：返回 Anthropic + 繼續領導 Claude Code（2025年8月至今）
- **說法：** 幾乎沒有公開討論這段插曲
- **行動：** 回來後繼續推進 Claude Code 的 agentic 功能、MCP 協議、hooks 系統
- **信號：** 這段插曲後他的公開發聲更加聚焦；Cursor 插曲反而強化了「他選擇留守 Claude Code」的形象

---

## 二、設計決策模式：Latent Demand 識別法

### 核心方法論
**問題：** 人們現在在用什麼錯誤工具來完成這件事？

**應用案例：**

| 工具 | 識別到的 Latent Demand | 正確工具 |
|------|----------------------|---------|
| json-schema-to-typescript | 有 JSON Schema 但需要 TypeScript 類型的工程師在手動維護兩份 | 自動轉換工具 |
| undux | Redux 太重，但工程師仍在用它做簡單狀態管理 | 輕量 Observable 方案 |
| Claude Code | 工程師在用 Copilot/ChatGPT 但每次都要離開終端機複製貼上 | 真正在終端機工作的 AI |

**識別 Latent Demand 的三個問題：**
1. 他們現在怎麼做這件事？（工作流調查）
2. 哪裡最讓他們煩躁？（痛點定位）
3. 如果有正確工具，他們願意換嗎？（需求驗證）

---

## 三、技術決策模式

### TypeScript 嚴格模式（strict: true）
- **立場：** 從第一天就開啟，不討論
- **邏輯：** 早期的類型寬鬆到後來關不掉；遷移成本隨時間指數增長
- **「Always make sure that when you start a migration, you finish the migration.」**

### Type-Driven Development 優先
- **立場：** 先寫類型簽名，再寫實現
- **邏輯：** 類型簽名迫使你在寫代碼前思考資料的形狀；這個思考過程本身就是設計
- 比先寫實現後再加類型節省大量重構時間

### Claude Code 的終端機優先決策
- **立場：** 不做 GUI；堅持終端機介面
- **邏輯：** 工程師的工作已經在終端機——AI 工具應該來找工程師，不是讓工程師去適應 AI
- **Unix 哲學：** 做好一件事；可組合；文字介面

### Extensibility over Features
- **立場：** 先做好可延伸性（MCP、hooks），讓社群自己做功能
- **邏輯：** 預測所有用戶需求是不可能的；給他們建構塊（building blocks）比給預製功能更有價值

---

## 四、決策風格特徵

### 1. 工程實用主義（Engineering Pragmatism）
- 「正確但不實用」的解法在他看來就是錯誤的解法
- 對「學術上優雅但工程上複雜」有明顯不耐
- 追求「能跑的最簡單代碼」

### 2. 完成主義（Completionist approach to migrations）
- 不接受半成品狀態
- 「手術中途停下來」的比喻反映他對未完成遷移的態度
- 這也反映在 Claude Code 的 agent mode 設計：讓 AI 自主完成任務，而非每步問人

### 3. 以工程師為中心（Engineer-centric design）
- 每個產品決策都從「工程師的工作流是什麼」出發
- 不是「我覺得這樣更好」，是「工程師現在怎麼工作，我怎麼配合他們」

### 4. 靜默後深思（Low-noise, high-signal）
- 相對於同行（Karpathy 等），公開發言少
- 但每次發言都有具體內容（功能更新、設計說明、技術觀點）
- 不追熱點，不做空洞的行業評論

### 5. 高風險時刻的快速校正（Cursor 插曲）
- 快速承認決策錯誤（或至少意識到更好的選擇）
- 不為面子留在錯誤的位置
- 返回後低調重新投入，不過度解釋

---

## 五、公開表達的工程哲學

1. **Type-first, implementation-second** — 類型是設計的起點
2. **Latent demand over explicit demand** — 識別用戶用錯工具的地方
3. **Finish what you start** — 遷移必須完成
4. **Tools should meet engineers where they are** — AI 工具應配合工程師的工作流
5. **Extensibility enables a future you can't predict** — 可延伸性比功能完備更重要

---

## 主要來源
- SE Radio Episode 384（2020）
- Lenny's Newsletter Podcast（2026）
- Pragmatic Engineer Newsletter（2025）
- YC Lightcone（2025）
- https://github.com/bcherny
- 業界報導（多篇，2024-2026）
