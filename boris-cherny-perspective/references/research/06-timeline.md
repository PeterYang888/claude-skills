# Boris Cherny 生平時間軸調研報告

**調研時間：** 2026-05-20

---

## 一、生平基本資料

| 項目 | 資料 | 可信度 |
|------|------|--------|
| 出生地 | 敖德薩（Odessa），烏克蘭（當時為蘇聯） | ✅ 高（本人提及） |
| 家族背景 | 祖父是蘇聯時期的打孔卡（punch-card）程序員 | ✅ 高 |
| 移民時間 | 約1995年，年幼時隨家人移居美國 | ✅ 高 |
| 就讀大學 | 加州大學聖地亞哥分校（UCSD） | ✅ 高 |
| 大學專業 | ⚠️ 待確認：部分資料說「電腦科學」，部分說「經濟學（可能中途輟學）」 | ⚠️ 低 |
| 現國籍 | 美國 | ✅ 高 |

**重要背景：** 祖父是蘇聯打孔卡程序員——對計算機作為工具的親切感可能從小就通過家庭文化傳承。

---

## 二、職涯時間軸

| 時間 | 事件 | 重要性 |
|------|------|--------|
| ~1995 | 移居美國（年幼，約5-10歲）| 移民背景；成長於美國工程師文化 |
| ~2010-2015 | 多個早期新創工作（具體公司待確認） | 積累工程經驗；建立 TypeScript 技術基礎 |
| 2015 | 發布 json-schema-to-typescript（GitHub）| 解決前端工程類型定義痛點；3,300+ stars |
| 2017 | 加入 Meta（Facebook），職稱：前端工程師（IC4）| 大規模工程環境 |
| 2019 | 出版《Programming TypeScript》（O'Reilly）| 確立 TypeScript 教育者地位；Goodreads 4.15/5 |
| 2020 | SE Radio Episode 384（TypeScript 深度訪談）| 第一個重要公開訪談 |
| 2020 | 發布 undux（輕量 React 狀態管理）| 1,600+ GitHub stars |
| 2017-2024 | Meta 晉升路徑：IC4 → IC8（7年）| 達到 Meta 最高個人貢獻者級別 |
| **2024年9月** | **加入 Anthropic，開始創建 Claude Code** | 最重要的職涯轉折點 |
| 2024年底-2025年 | Claude Code 公開發布，快速獲得工程師社群採用 | AI 工具市場重要節點 |
| **2025年7月** | **短暫加入 Cursor（Chief Architect）** | ⚠️ 常被忽略的插曲 |
| **2025年7月~8月** | **約2週後返回 Anthropic** | 重新領導 Claude Code |
| 2025-2026 | Claude Code 持續演進：agentic mode、MCP、hooks 系統 | 確立 AI 編程工具標準 |
| **2026年5月** | **現任職位：Head of Claude Code，Anthropic** | 最新狀態 |

---

## 三、Meta 任職期間詳情（2017-2024）

### 晉升路徑
- IC4（入職）→ IC5 → IC6 → IC7 → IC8（7年）
- IC8 是 Meta 個人工程師路徑的最高等級（等同於傑出工程師 Distinguished Engineer 層級）

### 主要技術工作
- 大規模前端架構
- Flow 類型系統的使用和貢獻（**作為用戶**，非核心開發者）
- Hack 語言相關工作（Meta 的 PHP 方言）
- 開源工具開發（json-schema-to-typescript、undux）

### ⚠️ 澄清：Cherny 與 Flow 的關係
- Flow 的創建者：**Avik Chaudhuri、Basil Hosmer、Gabriel Levi**（Facebook 研究院）
- Cherny 是 Flow 的**重度用戶和貢獻者**，在 Meta 工作期間廣泛使用
- 他對 Flow vs TypeScript 的深度理解來自這段實際使用經驗
- **他從未是 Flow 的核心開發者**

---

## 四、Anthropic 時期詳情（2024-現在）

### 加入背景
- 2024年9月，從 Meta 加入 Anthropic
- 角色：創建 Claude Code（從零開始）
- 直接看到的機會：「工程師已經在用 AI 工具，但沒有人做一個真正在終端機工作的工具」

### Claude Code 發展史
| 時間 | 里程碑 |
|------|--------|
| 2024年9月-12月 | 內部開發 Claude Code 初版 |
| 2025年初 | Claude Code 公開發布（測試版）|
| 2025年 | Agentic mode 強化 |
| 2025年 | MCP（Model Context Protocol）整合 |
| 2025年 | Hooks 系統推出 |
| 2026年 | 成為主流 AI 編程工具；「sub-agents」功能強化 |

### Cursor 插曲（2025年7月）
- **離開：** 加入 Cursor 擔任 Chief Architect
- **返回：** 約2週後回到 Anthropic
- **公開說明：** 幾乎沒有
- **影響：** 短期社群質疑，長期反而強化了「他選擇 Claude Code」的形象

---

## 五、常見誤記整理

| 誤記 | 正確資訊 |
|------|---------|
| 「Boris Cherny 曾在 Stripe 工作」 | **從未在 Stripe 工作**；此誤記可能因 TypeScript 生態重疊造成 |
| 「他是 Facebook Flow 的創建者」 | **Flow 創建者是 Avik Chaudhuri 等人**；Cherny 是 Flow 的用戶/貢獻者 |
| 「他大學主修電腦科學」 | **主修待確認**；部分資料說經濟學（可能未完成） |
| 「他一直在 Anthropic」 | **2025年7月短暫加入 Cursor**，約2週後返回 |
| 「Programming TypeScript 是入門書」 | **面向有 JS 基礎的工程師**，不是入門教材 |

---

## 六、個人背景對思維的影響

- **蘇聯背景家庭 → 美國成長：** 移民經歷可能強化對「工具讓更多人能做事情」的敏感度
- **祖父的打孔卡背景：** 計算機不是神秘物，是工具——從小就去神秘化
- **UCSD 非頂尖工程科系（待確認）→ Meta IC8：** 職業軌跡強調工程能力本身，而非名校光環
- **Meta 7年 IC 路徑：** 選擇個人工程師路徑而非管理路徑，反映對技術深度的偏好
- **Cursor 插曲快速返回：** 使命感勝過職位吸引力——在 Anthropic 做 Claude Code 的使命感更強

---

## 主要來源
- https://www.se-radio.net/2020/01/episode-384-boris-cherny-on-typescript/
- https://www.oreilly.com/library/view/programming-typescript/9781492037644/
- https://github.com/bcherny
- Lenny's Newsletter Podcast（2026）
- Pragmatic Engineer Newsletter（2025）
- 業界報導（多篇，2024-2026）
- LinkedIn 公開資料（部分待確認）
