# Boris Cherny 著作與公開輸出調研報告

**調研時間：** 2026-05-20

---

## 一、主要著作

### 《Programming TypeScript》（O'Reilly Media, 2019）

- **副標題：** Making Your JavaScript Applications Scale
- **定位：** 工程師導向的 TypeScript 深度教材；非入門書，面向有 JS 基礎的開發者
- **評分：** Goodreads 4.15/5（約1,200+評分）
- **核心教學方法：Type-Driven Development**
  - 「先寫類型，再填值」（sketch type signatures first, then fill in values）
  - 把類型系統當設計工具，而非注釋工具
- **章節結構特色：**
  - 從 JS 痛點出發，說明 TS 解決了什麼
  - 涵蓋：類型推論、泛型、型態守衛（type guards）、條件類型、mapped types
  - 進階主題：協變/逆變（co/contravariance）、嚴格性配置、聲明文件
- **寫作風格：** 口語親切，大量對話式說明；技術術語精確但不炫耀
- **影響力：** 被多所大學和公司採用為 TypeScript 標準教材

---

## 二、部落格與文章

### Medium / 個人網站文章（精選）

| 標題 | 核心觀點 | 可信度 |
|------|---------|--------|
| 「Introducing Undux」 | 輕量 Redux 替代方案；用 Observable 做狀態管理 | ✅ 高（GitHub 有對應 repo） |
| TypeScript 相關教學文章 | 類型系統深度解析 | ✅ 高 |

---

## 三、主要開源項目

### json-schema-to-typescript
- **用途：** 將 JSON Schema 自動轉換為 TypeScript 類型定義
- **GitHub Stars：** 3,300+（他最受歡迎的開源項目）
- **發布時間：** 2015年左右（Meta 任職期間）
- **背景：** 解決「有 JSON Schema 但需要 TypeScript 類型」這個極常見的工程痛點
- **使用廣泛度：** 每週下載量數十萬，被大量企業前端工程採用

### undux
- **用途：** 輕量 React 狀態管理庫（Redux 替代方案）
- **GitHub Stars：** 1,600+
- **設計哲學：** 盡可能簡單；用 Observable 取代 Redux 的 action/reducer 複雜度
- **現狀：** 已歸檔（archived）；Redux Toolkit 普及後需求減少

### 其他貢獻
- tslib（TypeScript 工具庫貢獻者）
- GitHub handle：bcherny
- GitHub followers：8,400+

---

## 四、Claude Code（最重要的作品）

### 創建過程
- **時間：** 2024年9月加入 Anthropic 後，從頭建構 Claude Code
- **定位：** AI 原生的終端機編程工具；讓 Claude 能夠直接操作代碼庫
- **Cherny 的角色：** 創建者（Creator）+ 早期負責人，現為 Head of Claude Code
- **設計思路：** 「工程師已經在終端機工作，為什麼 AI 工具要強迫他們去 IDE？」

### 產品哲學
- 以 Unix 哲學為基礎：可組合、文字介面、尊重現有工具鏈
- 「latent demand」原則：工程師已在用 AI 輔助編程，但工具不對；Claude Code 是給他們正確工具
- 堅持可延伸性（extensibility）：MCP 協議、hooks、自定義代理

---

## 五、訪談與演講

| 媒體 | 時間 | 主題 | 重要語錄 |
|------|------|------|---------|
| SE Radio Episode 384 | 2020 | TypeScript 深度訪談 | Type-Driven Development 的完整闡述 |
| Lenny's Newsletter Podcast | 2026 | Claude Code 的誕生與未來 | 「coding is largely solved」 |
| YC Lightcone Podcast | 2025 | AI 編程工具與工程師的未來 | 關於工程師角色轉型 |
| Pragmatic Engineer Newsletter | 2025 | Claude Code 產品設計理念 | 延伸性設計哲學 |

---

## 六、Twitter/X 存在感

- **Handle：** @bcherny
- **風格：** 技術性為主，分享 Claude Code 更新、TypeScript 技巧、產品思考
- **發文頻率：** 中等（相比 Karpathy 低調許多）
- **粉絲數：** 約數萬（具體數字待確認）

---

## 主要來源
- https://www.oreilly.com/library/view/programming-typescript/9781492037644/
- https://github.com/bcherny/json-schema-to-typescript
- https://github.com/bcherny/undux
- https://www.se-radio.net/2020/01/episode-384-boris-cherny-on-typescript/
- https://www.lennysnewsletter.com/p/inside-claude-code（2026年訪談）
- https://goodreads.com/book/show/45362865-programming-typescript
