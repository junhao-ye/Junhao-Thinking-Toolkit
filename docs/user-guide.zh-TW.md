# Junhao-Thinking-Toolkit 使用說明書

**繁體中文** · [简体中文](user-guide.zh-CN.md) · [English](user-guide.en.md) · [日本語](user-guide.ja.md)

[返回繁體中文 README](../README.md)

## 安裝與更新

1. 從儲存庫取得完整的 [`skills/junhao-thinking-toolkit`](../skills/junhao-thinking-toolkit) 資料夾，保留 `SKILL.md` 和同層的 `references/`。
2. 把整個資料夾複製到 Agent 的技能目錄。以 Codex 為例，安裝後應可在 `~/.codex/skills/junhao-thinking-toolkit/SKILL.md` 找到入口檔。在 Windows 中，`~` 代表你的使用者家目錄。
3. 開啟新對話，從技能清單選取 `junhao-thinking-toolkit`，或在請求中點名。先用一小段筆記試跑整理材料，確認回覆包含分組和原文線索。
4. 更新時，先保留自己修改過的檔案，再用新版的完整技能資料夾替換舊版，讓入口檔和參考檔維持同一版本。

## 提出第一個任務

交代你要推進的事、目前有哪些材料、限制是什麼，以及希望收到哪種產物。知道方法時可以點名，也可以讓工具箱依目的選擇。以下模板可直接改寫。

```text
請使用 junhao-thinking-toolkit。
我想釐清 [問題]，以便 [要做的決定或行動]。
可用材料是 [筆記、資料或連結]。限制是 [時間、預算或底線]。
請交付 [表格、檢查清單或分步引導]，並用繁體中文回答。
```

互動式方法每輪聚焦一個問題，答完再進下一步。已經準備好材料時，可以要求直接交付。若串接兩個方法，先說清楚第一個結果會如何用在第二個方法。

## 方法索引

### 四個輕量入口

| 方法 | 何時使用 | 會收到什麼 |
| --- | --- | --- |
| [整理材料](../skills/junhao-thinking-toolkit/references/organize-material.md) | 想整理筆記、聚焦重點或找重複模式 | 分組、原文依據，以及有待驗證的線索 |
| [假設檢驗](../skills/junhao-thinking-toolkit/references/solve-problem.md) | 想知道哪些前提左右方案成敗 | 關鍵假設、反例、替代解釋與驗證條件 |
| [逐步引導](../skills/junhao-thinking-toolkit/references/solve-problem.md) | 問題已清楚，想自己參與解題 | 當前一步、完成標準與一個幫助你往下做的問題 |
| [行動規劃](../skills/junhao-thinking-toolkit/references/make-decision.md) | 方向已定，需要安排執行 | 優先順序、時程、依賴、阻礙與第一步 |

### 十二種核心方法

| 方法 | 何時使用 | 會收到什麼 |
| --- | --- | --- |
| [蘇格拉底問診](../skills/junhao-thinking-toolkit/references/clarify-question.md) | 真正卡點還沒說清楚 | 每輪一問，收束成可回答的問題 |
| [雙層解釋](../skills/junhao-thinking-toolkit/references/learn-and-verify.md) | 想先建立直覺，再理解精確機制 | 直覺與專業兩層解釋、類比邊界與理解檢查 |
| [反向拆解](../skills/junhao-thinking-toolkit/references/learn-and-verify.md) | 想從現有成品學做法 | 可遷移的規律、操作清單與最小練習 |
| [橫縱分析](../skills/junhao-thinking-toolkit/references/learn-and-verify.md) | 想同時研究歷史演變與同類對象 | 時間線、橫向對照與未來路徑 |
| [事實核查](../skills/junhao-thinking-toolkit/references/learn-and-verify.md) | 想驗證可查證的說法或數字 | 逐項核實結果、來源、日期與推理缺口 |
| [專家會診](../skills/junhao-thinking-toolkit/references/solve-problem.md) | 同一問題需要互補的專業視角 | 各觀點的理由、風險、關鍵分歧與綜合判斷 |
| [第一性原理](../skills/junhao-thinking-toolkit/references/solve-problem.md) | 既有方案被慣例限制 | 從基本事實與限制重建的選項與驗證動作 |
| [跨領域借解](../skills/junhao-thinking-toolkit/references/solve-problem.md) | 慣用解法卡住，想找相似機制 | 可遷移的機制、適用條件與試驗 |
| [雙向鋼人／多選項比較](../skills/junhao-thinking-toolkit/references/make-decision.md) | 兩個或以上的選項難以取捨 | 兩案各自最強的論據，或多案的同準則比較 |
| [最小可逆實驗](../skills/junhao-thinking-toolkit/references/make-decision.md) | 關鍵未知可用短期、低成本行動驗證 | 實驗步驟、指標、繼續或停止門檻 |
| [天賦考古](../skills/junhao-thinking-toolkit/references/self-exploration.md) | 想從具體經驗找反覆出現的優勢 | 優勢假設、經歷證據與 30 天驗證 |
| [人生設計](../skills/junhao-thinking-toolkit/references/self-exploration.md) | 想比較幾條值得探索的未來方向 | 三個五年版本與本週可試的原型行動 |

## 可直接使用的範例

### 從筆記找模式

> 使用 junhao-thinking-toolkit 整理這 12 則客服筆記。按主題分組，重複轉述的事件合併計算，每個候選模式附上筆記編號和例外。最後標出一項最值得查證的線索。

你會得到有原文依據的模式清單。只有少數案例時，回覆應標成待驗證的線索。

### 先比較，再決定要不要試

> 使用 junhao-thinking-toolkit 比較兩個客服流程。底線是回覆品質，預算上限是每週 4 小時。先為兩個方案提出最強論據。若取捨取決於一項可以觀察的未知，再設計一週內可回退的試驗，寫出指標和停止門檻。

先讀比較結果。若還有會改變選擇的未知，試驗結果就可用來更新決策。

### 每輪自己解一步

> 使用 junhao-thinking-toolkit，逐步引導我找出這份轉換率計算的錯誤。每輪只給當前一步、完成標準和一個問題。等我回覆後再繼續。

若後來想直接看完整流程，可以請它整理已完成的步驟，接著列出剩餘步驟與檢查點。

## 判讀結果與常見問題

- **技能沒有出現在清單。** 確認 Agent 支援 Agent Skills、目前的執行環境能讀到技能目錄，且 `SKILL.md` 與 `references/` 位於同一個技能資料夾。再開一個新對話確認。
- **選錯方法或回覆太長。** 說明你要的產物，或直接指定方法和篇幅。例如「只做假設檢驗，給我一張表」。如果是純摘要、翻譯或簡單查詢，可以直接提出原任務。
- **回覆裡有待驗證的內容。** 區分素材陳述、已核實事實、推斷與價值取捨。需要查證時可要求一手來源與日期。缺少證據時，把結論保留為待驗證。
- **材料含敏感資訊或內嵌提示詞。** 分享前先移除個資、憑證與其他不必要的敏感內容。請求中寫清楚要如何處理附件，讓其中的提示詞以引用材料的方式分析。
- **涉及醫療、法律、重大財務或心理健康。** 可用工具箱整理問題與準備資料，把專業判斷交給合格專業人士。自我探索的輸出以可驗證的假設與行動為主。

需要了解方法的出處或維護方式時，可查看[來源與對照](../skills/junhao-thinking-toolkit/SOURCES.md)和[技能規格](../skills/junhao-thinking-toolkit/SPEC.md)。
