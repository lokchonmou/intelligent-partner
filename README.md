# 我的智能拍檔 · Intelligent Partner

**AI 是智力的引導，而不是智力的取代。**

一個以繁體中文編寫的 Agent Skill，支援共同思考、研究、學習及多步專案。按需要維護對話紀錄、學習筆記與計劃，保留人的判斷及可見的思考轉折。

An instruction-based Agent Skill for collaborative thinking, learning, evidence checking, and project delivery. It maintains logs, knowledge notes, and plans when needed, while keeping human judgment central.

## 適合甚麼任務？

- 與 AI 閱讀研究、檢查主張與證據，再修訂自己的理解。
- 把項目拆成可驗收的小步，留下測試及決策依據。
- 把多輪對話整合成可重讀、可交接的知識與現行計劃。

簡短問答不強制建立三份文件。學習時用提問、反例及分級提示保留認知掙扎；明確的執行任務直接完成，不機械地扣起答案。

## 核心方法

| 文件 | 保存甚麼 | 整理方式 |
|---|---|---|
| logging／對話紀錄 | 重要往返、決策、修訂理由 | 保留歷史與當時狀態 |
| notes／學習筆記 | 概念、來源、思考轉折與未解 | 按主題整合，保留理解形成的路徑 |
| plan／計劃 | 現行目標、規格、驗收與下一步 | 更新原位置，避免只在末尾追加 |

思考路徑：原有理解 → 問題／反例／證據 → 假設修正 → 新理解與理由 → 未解問題。只記公開表達及可檢查的協作依據，不補造人的思考。

重大決策、理解修正或測試後，更新受影響文件；收工、里程碑及交接時整體整理。這是在活躍任務中的維護規則，並非背景排程或永久記憶。

## 安裝

原始碼與安裝檔案：[lokchonmou/intelligent-partner](https://github.com/lokchonmou/intelligent-partner)。

### 支援 skills CLI 的 Agent

需要 Node.js／npx。在支援 skills CLI 的環境執行：

```bash
npx skills add lokchonmou/intelligent-partner --skill intelligent-partner
```

### Codex 本地安裝

下載倉庫，將 `skills/intelligent-partner` 整個資料夾放到你的 `~/.agents/skills/`。亦可請 `$skill-installer` 從公開 GitHub 倉庫的上述路徑安裝。載入後以 `$intelligent-partner` 啟動。

### ChatGPT

目前這份倉庫提供原始碼，未作官方插件目錄上架。ChatGPT 的分發形式及工作區權限與本地 CLI 不同；不要把上面的 npx 指令當成 ChatGPT 網頁版安裝方式。官方建議將可分發 Skill 包成 plugin，詳見 [Build skills](https://learn.chatgpt.com/docs/build-skills)。

## 開始使用

```text
使用 $intelligent-partner。我要審閱一份創新項目的草稿。
先讀我提供的現行文件，分清主張、證據、推論與未知。
協助我根據證據修訂構想；保留我的判斷與理由。
按需要維護 logging、notes、plan，階段結束時整理。
```

完成一個重要判斷後，你應能找回：原主張、支持範圍、人的判斷、修訂理由、未解事項。流暢文字或點頭不能單獨證明理解。

## 研發背景與目前證據

方法源於作者與 AI 的實際協作、教師與學生 AI 提問素養書籍規劃，以及對教育中人類主導權、認知努力與知識整理的關注。OECD 2026 的政策討論是設計參考，並非對本工具的認證。

作者已用此方法完成論文 review 及 Skill 自身的開發、修訂；已做基本結構檢查與有限情境試用。

- [OECD Digital Education Outlook 2026](https://www.oecd.org/en/publications/oecd-digital-education-outlook-2026_062a7394-en.html)
- [Reimagining Teaching in an Accelerating World：AI 與教育科技章節](https://www.oecd.org/en/publications/reimagining-teaching-in-an-accelerating-world_d0edfe8c-en/full-report/component-6.html)

## 能力與平台邊界

此 Skill 沒有重新訓練模型，也不安裝搜尋或文件工具。自動整理取決於 AI 遵守指令、實際讀到文件及具有讀寫能力；沒有工具時應提供可貼用內容並說明未保存。跨 Agent 行為仍需各自測試，不能因符合檔案格式就聲稱全面相容。

## 回饋與個人化

先套用，再根據真實任務一次修改一條規則。回報問題時提供預期行為、實際行為及可重現步驟；請先移除私人及學生資料。維持「人的判斷、證據驗收、思考路徑、按需文件」四個核心。

## 發布狀態與授權

2026-10-07：Skill 原始碼、文件規格、圖示及本 README 已公開至 GitHub。採用 [MIT License](LICENSE)，允許使用、複製、修改及再分發，須保留著作權與授權聲明；依 LICENSE 所載條件不提供保證。

目前以 GitHub 倉庫提供安裝；尚未建立版本 release、未確認 skills.sh 收錄，亦未提交 ChatGPT／Codex 官方插件目錄。

分享渠道：[skills.sh](https://skills.sh/) 支援以 GitHub 倉庫安裝及依安裝統計展示；ChatGPT／Codex 官方插件目錄需要另作插件打包與提交，不會因建立 GitHub 倉庫而自動上架。
