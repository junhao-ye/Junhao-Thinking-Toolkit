# Sources And Synthesis Record

## Source Inventory

| Source | Trust | Confidence | Contribution | Usage constraints |
| --- | --- | --- | --- | --- |
| [數字生命卡茲克，〈都 Agent 時代了，我還是想分享給你這 12 個我最常用的 Prompt〉](https://x.com/Khazix0918/status/2090726395035156964), 2026-08-21 | Primary author source | High | 5 大場景、12 種方法、互動節奏與原始輸出意圖 | 僅保留方法意圖與不可替代機制；執行文字重新作者化，不收錄大段逐字內容 |
| 使用者附圖 `Thinking-AI.jpg`，圖上署名 Dhaval Makwana | User-provided source | High for visible content | 10 種用 AI 輔助思考的方法與示例任務 | 依圖上內容適配。示例提示詞與視覺元素保留在原圖 |
| Local `skill-writer/SKILL.md` and routed references | Local authority | High | 新技能流程、參考架構、來源適配、描述優化、驗證 | Maintenance-only; not required at runtime |
| Local `adaptive-socratic-teacher/SKILL.md` | Neighboring implementation | Medium | 一次一問、回覆診斷、高風險教學邊界 | Used as local convention evidence, not a runtime dependency |
| Local `khazix-writer/SKILL.md` | Neighboring author-specific skill | Medium | 作者命名、歸因與中文觸發慣例 | Writing-style rules were intentionally excluded |

## Classification And Shape

- Skill class: `generic` — 結構化思考與自我探索工具箱。
- Primary execution shape: `router`。核心方法和輕量入口的觸發條件、互動節奏與產物不同。
- Secondary shape: `reference-backed-expert`。沿用情境分支，材料整理需要獨立的輸出契約，因此單列參考檔。
- Simpler shape rejected: `inline-guidance` 會迫使每次載入所有方法，增加誤路由、追問過度與上下文浪費。
- Portability: 純 Markdown 與相對路徑，沒有供應商專屬機制。

## Source Adaptation Decisions

| Decision | Status | Rationale |
| --- | --- | --- |
| 保留 5 類、12 方法與各方法的核心判斷機制 | Adopted | 這是原文最有辨識度且可重複使用的價值 |
| 將「複製貼上 Prompt」改為路由、流程、停止條件與輸出契約 | Adopted | Skill 需要在多輪與不同輸入下穩定執行 |
| 互動式方法維持一次只問一題 | Adopted | 防止問卷傾倒並允許依回答更新 |
| 原文指定的一萬字以上預設輸出 | Narrowed | 預設先給緊湊版本，只有使用者明確要求才擴寫，降低浪費與假精確 |
| 角色扮演成真實專家 | Replaced | 改為互補「專業視角」，不模仿或編造真實人物 |
| 自我探索中的心理學權威姿態 | Narrowed | 改為證據導向的優勢假設與人生原型，明確排除診斷與保證 |
| 原文敘事、推廣語、圖片、互動數據與逐字模板 | Omitted | 不改變 Runtime 決策；屬來源背景或受版權限制的表達 |
| 把附圖方法映射到既有方法與四個輕量入口 | Adopted | 用使用者想取得的產物選路由，保留原有核心方法與出處 |
| 照搬附圖示例的固定數量、版面與效益宣稱 | Omitted | 數量依使用者指定或路由預設。只提取能改變執行與交付的做法 |

## 附圖方法覆蓋

| 圖中方法 | 採用方式 |
| --- | --- |
| 01 倒出想法 | 整理材料按主題收斂觀察、想法與疑問 |
| 02 拆解複雜概念 | 雙層解釋加入機制步驟、具體例子與類比邊界 |
| 03 挑戰假設 | 假設檢驗列支持線索、替代解釋與可驗證條件 |
| 04 從多角度看問題 | 專家會診簡版並列不同立場與最重要分歧 |
| 05 組織資訊 | 整理材料依用途選擇大綱、表格或分層清單 |
| 06 發現模式與洞察 | 整理材料找跨記錄模式，保留反例與回查依據 |
| 07 做出更好的決策 | 雙向鋼人／多選項比較納入可能結果及改變排序的條件 |
| 08 一步步思考 | 逐步引導交付當前一步、完成標準與一個推進問題 |
| 09 減少思維雜訊 | 整理材料保留影響理解或決策的資訊 |
| 10 把想法化為行動 | 行動規劃整理任務、優先順序、時程、阻礙與第一步 |

## Coverage Matrix

| Dimension | Status | Implemented in |
| --- | --- | --- |
| Route categories and triggers | Complete | `SKILL.md` routing table |
| Ambiguous routes and fallback | Complete | one-primary-route rule, misroute recovery |
| Per-route execution contract | Complete | six files under `references/` |
| Interactive stop conditions | Complete | clarify and self-exploration references |
| Evidence and timeliness | Complete | common rules and learn/verify reference |
| Decision reversibility | Complete | solve and decision references |
| Self-exploration safety | Complete | self-exploration reference |
| Provider portability | Complete | no provider-specific mechanics |
| Automated behavioral evaluation | Deferred | requires future real usage examples |

## Trigger Test Set

Should trigger:

- 「我腦子很亂，先別給建議，幫我找出真正的問題。」
- 「同一個概念先講人話，再用專業版解釋。」
- 「拆解這個產品頁為什麼做得好，我想學它的方法。」
- 「從歷史演化和競品比較研究這家公司。」
- 「幫我核查這段文章的數據和推論。」
- 「找三個互補專業角度會診這個組織問題。」
- 「不要沿用行業慣例，從第一性原理重做。」
- 「其他產業有沒有解過類似的供需問題？」
- 「A、B 都有道理，幫我做最強的正反論證。」
- 「設計一個七天內能驗證需求的低成本實驗。」
- 「從我的經歷找可能被忽略的底層優勢。」
- 「我想設計三個完全不同的五年人生版本。」

新增與重疊案例：

| 請求 | 預期路由與檢查點 |
| --- | --- |
| 把這些碎念按主題整理，留下會影響決策的事 | 整理材料。保留例外與歧義，直接交付 |
| 四則客服記錄是否有重複問題？其中兩則指同一張單 | 整理材料。同一事件合併計算，附記錄依據 |
| 幫我挑戰「只要降價就會提高續約」的前提 | 假設檢驗。列替代解釋與能區分兩者的觀察 |
| 查證這份報告寫的「降價後續約率增加 20%」 | 事實核查。核對來源、比較基準與時間區間 |
| 給我五個角度看這個提案，含合理反方 | 專家會診簡版。列出五個有實質差異的立場 |
| 題目在這裡，請逐步引導我解，每輪一步 | 逐步引導。先交付當前步驟與一個問題 |
| 我想改善工作流程，但還不確定卡在哪裡 | 蘇格拉底問診。先釐清真正卡點 |
| 用我的目標比較三個方案的收益、風險與可能結果 | 多選項比較。使用共同準則，保留各選項 |
| 已決定採用 B，排出時程，但主管還沒給截止日 | 行動規劃。用相對時程，標示待確認期限 |

Should not trigger:

- 「台北現在幾點？」
- 「把這段話改得更通順。」
- 「幫我摘要這份會議紀錄。」
- 「用 SWOT 分析這家公司。」
- 「直接翻譯成英文。」
- 「替我寫一篇卡茲克風格的公眾號長文。」

## Gaps And Stopping Rationale

- Open gap: 尚無真實使用紀錄可評估誤路由率、對話中途退出與長報告品質。
- Next retrieval: 收集匿名正例、負例與修正案例後，加入 holdout 測試並調整描述或路由。
- Retrieval stopped after mapping all 10 visible methods to the existing implementation and the new routes. The image and installed toolkit resolve the requested adaptation. Live routing accuracy still requires representative usage examples.
