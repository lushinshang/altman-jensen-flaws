# Sam Altman 談黃仁勳可能回任輝達執行長：訪談片段導讀

Semafor「Silicon Valley & The World」活動上，Sam Altman 被問到黃仁勳可能回任輝達執行長的約 8 分鐘訪談片段導讀。導讀以 Altman 說了什麼為主，並整理主持人提到的輝達擔保、Anthropic 上市、晶片需求「重複計算」、供應鏈與資料中心公投，查證集中在文內一張對照表。

> 本導讀的研究、翻譯、撰稿、查證與審稿皆由 AI 模型完成，並非人類分析，未經人工逐句校稿；英文為 YouTube 機器自動字幕，未逐句對照原音。

## 檔案

| 檔案 | 說明 |
|---|---|
| `index.html` | 導讀長文頁，可直接用瀏覽器開啟 |
| `altman-jensen-flaws.md` | 正式 Markdown（由 `research/guide_src.md` 產生，時間戳連結由腳本依字幕 cue 計算） |
| `player.html` | 雙語字幕播放器（YouTube 內嵌；字幕隨播放同步；需連網才能載入影片） |
| `translation-zh.html` | 全文繁中譯文（非官方，AI 翻譯，依機器字幕） |
| `images/` | `hero-16x9.png`／`hero-9x16.png`（AI 生成封面，桌面與手機）、`og-hero.jpg`（分享預覽 1200×630）、`fig-timeline-zh.svg`／`fig-timeline-zh-mobile.svg`（八分鐘分段圖，桌面與手機）；`_src/` 為本機備用的 WebP，不公開 |
| `research/`、`qa/` | 查證帳本、審稿紀錄、建置腳本與版面檢查，僅留本機 |

封面為 AI 生成的示意圖（不是影片畫面，圖內沒有文字與真人臉）；分段圖是腳本依字幕時間與講者歸屬表繪製的 SVG。三個頁面的 `og:image` 都指向 `images/og-hero.jpg`。

## 原始資料

- 類型：影片（訪談片段，DRM News 頻道上傳；畫面標示為 Semafor 活動）
- 名稱：“Heroes Have Flaws” OpenAI's Sam Altman on Jensen Huang's Possible Return as Nvidia CEO | AI1N
- 網址：https://www.youtube.com/watch?v=RizP4UPzxDU（2026-11-16 上傳，495 秒，無章節）
- 字幕：`transcription/…RizP4UPzxDU.en-orig.srt`（YouTube 英文機器字幕，433 筆滾動字幕合併為 98 句 cue）。同目錄另有一份 `ar-orig`（阿拉伯文）字幕，來自 YouTube 的自動配音／翻譯軌，**不是原音語言**，未使用。

## 重要來源

- 一手：[Semafor 報導](https://www.semafor.com/article/11/16/2026/altman-says-he-has-personal-empathy-for-jensen-huang)、[輝達 CEO 異動公告](https://nvidianews.nvidia.com/news/nvidia-announces-ceo-transition)（2026-11-12）、[輝達 8-K（OpenAI 俄亥俄資料中心殘值擔保）](https://www.sec.gov/Archives/edgar/data/1045810/000104581026000069/nvda-20260817.htm)（2026-08-17）、[Anthropic IPO 官方網站](https://ipo.anthropic.com/)
- 二手：Route Fifty、Venable（資料中心公投）；Crypto Briefing（轉述韓國 Financial News 的三星「重複計算」報導）

資料截至 2026-11-17。

## 重要限制

- 只是約 8 分鐘片段，完整訪談約 30 分鐘；片段最後一句沒說完。
- 字幕沒有說話者標記，Altman 與主持人的歸屬依換人標記與內容判斷；存疑的 05:58–06:12（主持人）與 07:06 之後（Altman）另用 agy 聽音訊判斷換人時間並與影格交叉，結果支持原判斷（只有一支片段起點的前 3 秒出現矛盾，判斷是片段起點的誤判）；03:24 前後一句歸屬仍無法確認（正文未引用）。agy 只做得到換人判斷，沒有逐字核對；對照組只有 3 支短片、4 個換人點，樣本很小；結果只當線索。主持人姓名依 Semafor 文章為 Reed Albergotti，畫面無名牌。
- 三星「重複計算」報導只有單一二手來源；輝達「不再出貨給中國」未查證；公投數字為初步統計。
- 譯文、初譯與修詞都未逐句對照原音；「Lyft（字幕作 lift）」兩者同音、無法由音訊判斷，依上下文推定；「PCB laminate」「blue wave」等幾個詞已請 agy 聽音訊核對，與字幕一致（只當線索）。
- 封面 PNG 內含生成工具寫入的內容憑證（C2PA）標記，可讀出為 AI 生成；沒有使用者資訊。
- 三個頁面的 `og:image` 在本機版是相對路徑；發布時需以 `--base`（或 `PUBLISH_BASE`）重建成絕對網址，否則分享預覽抓不到圖。
- 分段圖只有一類歸屬（依字幕換人標記與內容判斷，存疑處已用影片核對）加一個「歸屬不確定的一句」圓圈（03:24）；核對過程見 `research/av_check.md`。
- 製作分工：初譯 agy（gemini-3.8-flash-high）、修詞與撰稿 Claude Sonnet 5.5、審稿（事實／編輯／終審）Sonnet 與 Opus、總編輯潤稿 Opus，完稿後另請總編輯（Opus）審上下文、語意與話題銜接；封面用 Codex imagegen 生成，分段圖為腳本繪製的 SVG；講者歸屬存疑處另用 agy（gemini-3.8-flash-high 為主，Hydrogen 作仲裁）聽音訊與影格核對。

## 狀態

僅本機完成，**未發布**：沒有建立 repo、沒有推送。
