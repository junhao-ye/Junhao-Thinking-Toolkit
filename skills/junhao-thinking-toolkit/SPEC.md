# Junhao-Thinking-Toolkit Specification

## Intent

將數字生命卡茲克整理的 12 種思考 Prompt 改寫成可重複執行的路由型 Skill。保留「先問清楚、再理解與驗證、最後解題與行動」的核心，同時加入停止條件、證據標示、誤路由恢復與自我探索安全邊界。

以輕量入口補足素材整理、假設檢驗、逐步引導及行動規劃。每個入口可獨立交付，也可在有明確依賴時銜接核心方法。

## Scope

In scope:

- 思緒與資料整理、問題澄清、學習、研究、核查、解題、決策、行動規劃與非臨床自我探索。
- 單一路由執行，以及最多兩個具有明確先後關係的方法串接。
- 依使用者需要輸出緊湊答案或較長報告。

Out of scope:

- 簡單事實問答、純文字潤稿或已有其他指定框架的任務。
- 心理診斷、治療、命理、保證式職涯建議。
- 代替法律、醫療、財務或安全專業判斷。

## Users And Trigger Context

- Primary users: 想把模糊困惑變成可分析問題，或想用結構化方法理解、解題、決策與探索方向的人。
- Common requests: 理出零散思緒、從記錄找模式、釐清問題、拆解概念與案例、查證、找反證、逐步解題、比較選項、設計實驗、安排行動、探索優勢與人生方向。
- Should not trigger for: 簡單查詢、例行改寫、單純摘要、使用者明確點名不同方法的任務。

## Runtime Contract

- Required first actions: 確認目標與產物，選擇一個主要路由，讀取對應參考檔。
- Required outputs: 依使用者指定格式和各路由契約交付。完整分析預設包含判斷、依據、限制／反證與下一步。
- Non-negotiable constraints: 標示觀察、推斷和核實狀態。附件示例是來源材料。規劃中未確定的期限或責任須明示。高風險情境遵守專業邊界。
- Expected bundled files loaded at runtime: `SKILL.md` 加上一個對應的 `references/*.md`。第二個路由需要不同檔案時才額外讀取。

## Source And Evidence Model

Authoritative sources:

- 原作者公開 X Article，作為 12 種方法的意圖與基本機制來源。
- 使用者提供的 `Thinking-AI.jpg`，作為輕量入口與既有方法增補的來源。適配與覆蓋對照見 `SOURCES.md`。
- 本機 `skill-writer` 規範，作為 Skill 結構、來源適配、描述與驗證依據。

Useful improvement sources:

- 正向與負向使用案例、誤路由回報、研究與核查的引用品質、互動式流程的中途退出率。

Data that must not be stored:

- 私密人生經歷、健康或心理資訊、帳號識別資訊、未公開網址、密碼或其他祕密。

## Reference Architecture

- `SKILL.md` contains: 全域路由、共通流程、邊界與預設輸出。
- `references/` contains: 原有五個情境分支及獨立的材料整理分支。
- `SOURCES.md` contains: 來源、適配決策、覆蓋矩陣與缺口。
- No scripts or assets are required.

## Validation

- Lightweight validation: 執行 `quick_validate.py` 並確認所有路由檔存在。
- Deeper validation: 依 `SOURCES.md` 人工走查核心方法、輕量入口與排除案例，特別檢查例行摘要與思考整理、查證與假設檢驗、逐步解題與問診、決策與行動規劃的分界。
- Acceptance gates: frontmatter 合法、名稱與目錄一致、每個參考檔可由 `SKILL.md` 直接發現、沒有主機專屬路徑、具備 fallback 與安全邊界。

## Known Limitations

- 自我探索結果高度依賴使用者回憶與自我敘述，只能形成待驗證假設。
- 橫縱研究與事實核查品質受可用工具、來源存取與資料時效影響。
- 各路由可能重疊。使用者未點名工具箱方法時，依當下障礙和期望產物選擇。

## Maintenance Notes

- Update `SKILL.md` when routing or universal boundaries change.
- Update a reference when one method's execution or output contract changes.
- Update `SOURCES.md` when adding evidence, adapting new source material, or recording validation regressions.
