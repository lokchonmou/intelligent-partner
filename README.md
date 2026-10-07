# 我的智能拍檔 · Intelligent Partner

**AI 是智力的引導，而不是智力的取代。**

**AI should guide human intelligence, rather than replace it.**

一個以繁體中文編寫的 Agent Skill，支援共同思考、研究、學習及多步專案。按需要維護對話紀錄、學習筆記與計劃，保留人的判斷及可見的思考轉折。

An Agent Skill written in Traditional Chinese for collaborative thinking, research, learning, and multi-step projects. It maintains conversation logs, learning notes, and plans when needed, while preserving human judgment and visible changes in understanding.

## 適合甚麼任務？ / Suitable Tasks

與 AI 閱讀研究、檢查主張與證據，再修訂自己的理解；把項目拆成可驗收的小步，留下測試及決策依據；把多輪對話整合成可重讀、可交接的知識與現行計劃。

Read research with AI, examine claims and evidence, and revise your understanding. Break projects into small, verifiable steps and retain the basis for tests and decisions. Turn extended conversations into knowledge and current plans that can be revisited or handed over.

簡短問答不強制建立三份文件。學習時用提問、反例及分級提示保留認知掙扎；明確的執行任務直接完成，不機械地扣起答案。

Brief questions do not require three documents. During learning, questions, counterexamples, and graduated hints preserve cognitive struggle. For clearly defined execution tasks, the AI completes the work without mechanically withholding answers.

## 核心方法 / Core Method

**對話紀錄（logging）**保存重要往返、決策及修訂理由，保留歷史與當時狀態。

**Conversation logs** preserve key exchanges, decisions, and reasons for revisions, including the history and status at each stage.

**學習筆記（notes）**按主題整合概念、來源、思考轉折與未解問題，保留理解形成的路徑。

**Learning notes** organize concepts, sources, changes in thinking, and unresolved questions by topic, preserving how understanding developed.

**計劃（plan）**維持現行目標、規格、驗收與下一步，直接更新相關位置，避免只在末尾追加補充。

**Plans** maintain current goals, requirements, acceptance criteria, and next steps. Relevant sections are updated directly, rather than leaving revisions as appendices at the end.

思考路徑：原有理解 → 問題／反例／證據 → 假設修正 → 新理解與理由 → 未解問題。只記公開表達及可檢查的協作依據，不補造人的思考。

Thinking pathway: initial understanding → question, counterexample, or evidence → revised assumptions → new understanding and reasons → unresolved questions. Record only what the person expresses and what can be checked in the collaboration; do not invent their thinking.

重大決策、理解修正或測試後，更新受影響文件；收工、里程碑及交接時整體整理。這是在活躍任務中的維護規則，並非背景排程或永久記憶。

Update affected documents after significant decisions, changes in understanding, or tests. Consolidate them at session endings, milestones, and handovers. This maintenance happens during active tasks; it is not background scheduling or permanent memory.

## 安裝 / Installation

原始碼與安裝檔案：[lokchonmou/intelligent-partner](https://github.com/lokchonmou/intelligent-partner)。

Source code and skill files: [lokchonmou/intelligent-partner](https://github.com/lokchonmou/intelligent-partner).

### 支援 skills CLI 的 Agent / Agents Supporting the Skills CLI

需要 Node.js／npx。在支援 skills CLI 的環境執行以下指令。

You need Node.js and npx. Run the following command in an environment that supports the skills CLI.

```bash
npx skills add lokchonmou/intelligent-partner --skill intelligent-partner
```

### Codex 本地安裝 / Local Installation in Codex

下載倉庫，將 `skills/intelligent-partner` 整個資料夾放到你的 `~/.agents/skills/`。亦可請 `$skill-installer` 從公開 GitHub 倉庫的上述路徑安裝。載入後以 `$intelligent-partner` 啟動。

Download the repository and copy the entire `skills/intelligent-partner` folder into `~/.agents/skills/`. Alternatively, ask `$skill-installer` to install it from that path in the public GitHub repository. Once loaded, invoke it with `$intelligent-partner`.

### ChatGPT

目前倉庫提供原始碼，尚未上架官方插件目錄。ChatGPT 的分發形式及工作區權限與本地 CLI 不同；上述 npx 指令並非 ChatGPT 網頁版安裝方式。官方建議將可分發 Skill 包成 plugin，詳見 [Build skills](https://learn.chatgpt.com/docs/build-skills)。

The repository currently provides source files and is not listed in the official plugin directory. ChatGPT distribution and workspace permissions differ from local CLI installation; the npx command above does not install a skill in ChatGPT on the web. Official guidance recommends packaging a distributable skill as a plugin. See [Build skills](https://learn.chatgpt.com/docs/build-skills).

## 開始使用 / Getting Started

你可以用以下提示開始審閱創新項目的草稿。

Use the following prompt to start reviewing a draft for an innovation project.

```text
使用 $intelligent-partner。我要審閱一份創新項目的草稿。
先讀我提供的現行文件，分清主張、證據、推論與未知。
協助我根據證據修訂構想；保留我的判斷與理由。
按需要維護 logging、notes、plan，階段結束時整理。
```

英文提示：

English prompt:

```text
Use $intelligent-partner. I want to review a draft for an innovation project.
First read the current documents I provide. Distinguish claims, evidence,
inferences, and unknowns. Help me revise the idea based on evidence,
preserving my judgment and reasons. Maintain logs, notes, and plans
as needed, and consolidate them at the end of the stage.
```

完成一個重要判斷後，你應能找回：原主張、支持範圍、人的判斷、修訂理由、未解事項。流暢文字或點頭不能單獨證明理解。

After an important decision, you should be able to recover the original claim, the scope of supporting evidence, the person's judgment, the reasons for revision, and unresolved issues. Fluent writing or agreement alone does not demonstrate understanding.

## 研發背景與目前證據 / Development Background and Current Evidence

方法源於作者與 AI 的實際協作、教師與學生 AI 提問素養書籍規劃，以及對教育中人類主導權、認知努力與知識整理的關注。OECD 2026 的政策討論是設計參考，並非對本工具的認證。

The method grew from the author's practical collaboration with AI, plans for a book on AI questioning literacy for teachers and students, and concerns about human agency, cognitive effort, and knowledge organization in education. OECD's 2026 policy discussions inform the design; they do not certify or endorse this tool.

作者已用此方法完成論文 review 及 Skill 自身的開發、修訂；已做基本結構檢查與有限情境試用。

The author has used this method to complete a paper review and to develop and revise the skill itself. Basic structural checks and limited scenario trials have been conducted.

相關參考資料：

Related references:

- [OECD Digital Education Outlook 2026](https://www.oecd.org/en/publications/oecd-digital-education-outlook-2026_062a7394-en.html)
- [Reimagining Teaching in an Accelerating World — AI and education technology chapter](https://www.oecd.org/en/publications/reimagining-teaching-in-an-accelerating-world_d0edfe8c-en/full-report/component-6.html)

## 能力與平台邊界 / Capabilities and Platform Limits

此 Skill 沒有重新訓練模型，也不安裝搜尋或文件工具。自動整理取決於 AI 遵守指令、實際讀到文件及具有讀寫能力；沒有工具時應提供可貼用內容並說明未保存。跨 Agent 行為仍需各自測試，不能因符合檔案格式就聲稱全面相容。

This skill does not retrain a model or install search or file tools. Automatic organization depends on the AI following instructions, actually accessing the documents, and having read and write capabilities. Without those tools, it should provide text that can be copied and clearly state that nothing was saved. Behavior across agents still needs separate testing; a valid file format does not establish universal compatibility.

## 回饋與個人化 / Feedback and Personalization

先套用，再根據真實任務一次修改一條規則。回報問題時提供預期行為、實際行為及可重現步驟；請先移除私人及學生資料。維持「人的判斷、證據驗收、思考路徑、按需文件」四個核心。

Start with the skill as provided, then adjust one rule at a time using real tasks. When reporting a problem, describe the expected behavior, actual behavior, and steps to reproduce it; remove private and student information first. Preserve the four core principles: human judgment, evidence-based verification, thinking pathways, and documents created as needed.
