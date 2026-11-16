# 知識庫操作日誌 (`log.md`)

> 本文件為 Append-only（僅追加）的時間軸紀錄，記錄知識庫所有的 `ingest`（消化來源）、`query`（提問歸檔）與 `lint`（健康檢查）操作。
> 標準標題格式：`## [YYYY-MM-DD] <ingest|query|lint|init> | <標題>`（可使用 `grep "^## \[" log.md | tail -5` 快速檢視最近 5 筆操作）。

---

## [2026-11-16] init | 初始化金融與產業研究 LLM Wiki 知識庫
- **操作內容**：依據 Karpathy LLM Wiki 架構建立三層知識庫結構（`raw/`、`wiki/`、`AGENTS.md`/`agent.md`）。
- **新增檔案**：
  - `AGENTS.md` (`agent.md`)：定義全自動 Ingest / Query / Lint 流程、Obsidian `[[WikiLinks]]` 規範、矛盾與觀點演進追蹤機制。
  - `index.md`：建立公司、產業、概念、競品對比、原始來源五大分類索引。
  - `wiki/overview.md`：建立全局投資論點與產業版圖總覽頁。
  - `wiki/_templates/`：建立 `company.md`、`industry.md`、`concept.md`、`comparison.md`、`source-summary.md` 五個標準模板。

---

## [2026-11-16] ingest | Blanchard Macroeconomics Ch.2 - A Tour of the Book (`raw/Chap-2.pdf`)
- **原始來源**：`raw/Chap-2.pdf`（共 71 頁，含台灣行政院主計總處國民所得/失業定義補充、CPI vs. PCE 補充及課堂手寫筆記）
- **新建來源摘要頁（1 頁）**：
  - `wiki/sources/source-blanchard-chap-2.md`
- **新建概念頁面（5 頁）**：
  - `wiki/concepts/gdp-and-national-income-accounting.md`
  - `wiki/concepts/unemployment-and-labor-market-indicators.md`
  - `wiki/concepts/inflation-and-price-indexes.md`
  - `wiki/concepts/okuns-law-and-phillips-curve.md`
  - `wiki/concepts/macroeconomic-time-horizons.md`
- **新建專題對比頁（2 頁）**：
  - `wiki/comparisons/fixed-base-vs-chain-linked-gdp.md`
  - `wiki/comparisons/cpi-vs-pce-vs-gdp-deflator.md`
- **更新頁面（2 頁）**：
  - `wiki/overview.md`：新增 Ch.2–Ch.20 總體經濟四維度章節藍圖與三大實證論點（台美歐肯係數差異、ICT 跌價與連鎖法、Fed 採用 PCE 之邏輯）。
  - `index.md`：同步更新 8 個新建/更新頁面的分類索引與摘要。

---

## [2026-11-16] ingest | Blanchard Macroeconomics Ch.3 - The Goods Market (`raw/Chap-3.pdf`)
- **原始來源**：`raw/Chap-3.pdf`（共 46 頁，含台灣與美國 GDP 支出比重對比、三種乘數推導、節儉矛盾與加速效果）
- **前置檢查（Gate 1）**：驗算 `IS` 曲線代數推導練習（$C=100+0.75Y_D, I=50-25i, G=T=50 \implies Y = 650 - 100i$）與平衡預算乘數（$\frac{1-c_1}{1-c_1} = 1$）無誤；並標記「固定投資 $I=\bar{I}$」與「內生加速投資 $I=I(Y)$」下節儉矛盾對總儲蓄結論之差異。
- **新建/更新頁面**：
  - 新建 `wiki/sources/source-blanchard-chap-3.md`
  - 新建 `wiki/concepts/goods-market-and-multiplier.md`
  - 更新 `wiki/concepts/gdp-and-national-income-accounting.md`（新增台美支出面 GDP 組成結構表，`source_count` 升至 2）

---

## [2026-11-16] ingest | Blanchard Macroeconomics Ch.4 - Financial Markets (`raw/Chap-4.pdf`)
- **原始來源**：`raw/Chap-4.pdf`（共 46 頁，含存量/流量區辨、公開市場操作 OMO、貨幣乘數、流動性陷阱、台灣 M1A/M1B/M2 與 Fed IOR/ON RRP 新工具）
- **前置檢查（Gate 1）**：驗算貼現債券價格與利率公式（$i = \frac{\$100-\$P_B}{\$P_B}$）及兩種貨幣乘數公式（無通貨時 $\frac{1}{\theta}$，含通貨時 $\frac{1}{c+\theta(1-c)}$，手寫等比級數推導驗證一致）。
- **新建/更新頁面**：
  - 新建 `wiki/sources/source-blanchard-chap-4.md`
  - 新建 `wiki/concepts/money-market-and-monetary-policy.md`

---

## [2026-11-16] ingest | Blanchard Macroeconomics Ch.5 - Goods and Financial Markets: The IS-LM Model (`raw/Chap-5.pdf`)
- **原始來源**：`raw/Chap-5.pdf`（共 63 頁，含內生投資 IS 曲線、水平 vs. 正斜率 LM 曲線、全微分斜率與投資利率彈性、排擠效果、1990s 與 2001 政策組合案例）
- **前置檢查（Gate 1）— 抓出跨章節數據衝突**：
  - 比對發現 `Chap-5.pdf` Slide 48（依 BEA 修正後數據指出 **2001 Q2 實質 GDP 為小幅正成長**，未連續兩季負成長）與先前 `Chap-2.pdf` Slide 22（依初版數據稱 **2001 Q1–Q3 連續三季負成長**）存在數據修正衝突！已於 `wiki/concepts/gdp-and-national-income-accounting.md` 加入 `[!WARNING] 觀點分歧 / 數據衝突` 區塊完整記錄。
- **新建/更新頁面**：
  - 新建 `wiki/sources/source-blanchard-chap-5.md`
  - 新建 `wiki/concepts/is-lm-model-and-policy-mix.md`
  - 更新 `wiki/concepts/gdp-and-national-income-accounting.md`（`source_count` 升至 3）

---

## [2026-11-16] ingest | Blanchard Macroeconomics Ch.6 - Financial Markets II: The Extended IS-LM Model (`raw/Chap-6.pdf`)
- **原始來源**：`raw/Chap-6.pdf`（共 39 頁，含費雪方程式、風險溢酬 $x$、銀行槓桿與擠兌、延伸型 IS-LM、中性利率 $r^*$ 與 2008 次貸危機 MBS/CDO/SIV/TARP/QE）
- **前置檢查（Gate 1）**：驗算費雪方程式精確式與近似式（$1+r_t = \frac{1+i_t}{1+\pi_{t+1}^e} \implies r_t \approx i_t - \pi_{t+1}^e$）、風險溢酬公式（$x = \frac{(1+i)p}{1-p}$）及銀行資本比率/槓桿率（$20/100=20\%, 100/20=5$）無誤。
- **新建/更新頁面**：
  - 新建 `wiki/sources/source-blanchard-chap-6.md`
  - 新建 `wiki/concepts/extended-is-lm-and-financial-crisis.md`
  - 新建 `wiki/comparisons/fiscal-vs-monetary-policy-in-is-lm.md`
  - 更新 `wiki/overview.md` 與 `index.md`（完成 5 篇核心章節 Ingest，總計 18 個知識庫頁面）

---

## [2026-11-16] lint | 知識庫健康檢查與教學簡報前置審核 (Gate 2)
- **雙向連結與孤島檢查**：掃描 `wiki/` 下全數 18 個頁面（`overview.md` + 9 個 `concepts/` + 3 個 `comparisons/` + 5 個 `sources/`），所有 `[[WikiLinks]]` 均雙向連通，無孤島頁（Orphan pages）或懸空連結。
- **跨頁矛盾與勘誤一致性檢查**：
  1. `Chap-2` p.31 連鎖法表格算式印刷錯誤（`30` 修正為 `60`）已於 `source-blanchard-chap-2.md` 與 `overview.md` 一致標註。
  2. `Chap-2` vs. `Chap-5` 關於 2001 美國衰退 Q2 GDP 成長率之初版與修正版差異，已於 `gdp-and-national-income-accounting.md` 標註 `[!WARNING]`。
  3. `Chap-3` 固定投資 vs. 加速投資下之節儉矛盾結論差異，已於 `goods-market-and-multiplier.md` 標註 `[!WARNING]`。
- **結論**：知識庫通過 Gate 2 健康檢查，可作為唯一事實來源編譯教學型 HTML 簡報（`slides.html`）。

---

## [2026-11-16] slides | 編譯並產出教學型 HTML 簡報 (`slides.html`) (Gate 3)
- **知識來源**：查詢 `index.md`、`wiki/overview.md`、9 個 `wiki/concepts/` 頁面與 3 個 `wiki/comparisons/` 頁面。
- **產出檔案**：`slides.html`（共 10 頁互動式教學投影片，內建凱因斯乘數互動滑桿模擬器、IS-LM 政策衝擊動態 SVG 模擬器、章節目錄抽屜與鍵盤方向鍵導覽）。
- **Gate 3 檢查紀錄**：
  1. **Wiki 節點明確對應檢查**：第 1～10 頁投影片底部皆已附上對應之 `[[Wiki 頁面]]` 標籤與原始 PDF 頁碼範圍，100% 源自 Wiki 知識庫。
  2. **教學結構檢查**：從「三大體溫計（GDP/失業/通膨）」→「商品市場與乘數」→「金融市場與流動性陷阱」→「IS-LM 模型」→「延伸型 IS-LM 與 2008 金融海嘯」循序漸進，適合零基礎讀者理解。

---

## [2026-11-16] slides | 依使用者回饋重構 18 頁米色極簡中英雙語教學簡報 (`slides.html`) (Gate 3 Re-check)
- **需求對齊調整**：
  1. **目標受眾**：鎖定「完全沒學過經濟學的大學生与一般大眾」，移除複雜 IS-LM 圖形與微積分推導，改以生活案例（鋼鐵與汽車、買新房算投資、牛肉麵看通膨/通縮、蘋果與橘子看物價指數偏誤）引導。
  2. **語言與視覺**：採用溫暖米色紙感極簡排版（留白 $\ge 35\%$）、中英雙語標題與核心術語對照，將內容拆細為 **18 頁（每頁 1 個主觀念 + 1 個生活案例或對照表）**。
  3. **互動與 5 篇來源對應**：於第 5 頁內建「生活消費連鎖放大試算器（MPC 乘數）」、第 16 頁內建「存款實質購買力計算機（費雪方程式）」，自然串聯 `Chap-2` 至 `Chap-6` 全部 5 篇 Wiki 來源。

---

## [2026-11-16] slides | 新增 `slide-outline.md` 大綱檢查節點並編譯 16 頁可直接編輯版 `slides.html`
- **Workflow Graph 升級**：
  - 將「大綱與語言風格確認（Outline Gate）」提前至生成 HTML 之前，先產出 `slide-outline.md`（16 頁純繁體中文標題與小標，拿掉所有冗餘英文副標題與標籤）。
  - 大綱確認通過後，一對一編譯為 `slides.html`，並於右上角導覽列內建 **「✎ 編輯文字模式（`contenteditable`）」** 與 **「💾 儲存下載 HTML」** 按鈕，支援在瀏覽器中直接點擊任何文字進行刪除、修改與匯出存檔。


---

## [2026-11-16] ingest | Blanchard Macroeconomics Ch.7–Ch.11 (共 5 篇、234 頁 PDF) (Gate 1 & Gate 2)
- **原始來源**：
  1. `raw/Chap-7.pdf`（49 頁）：勞動市場（WS-PS 模型、效率工資、亨利·福特日薪 5 美元案例、自然失業率 $u_n$）
  2. `raw/Chap-8.pdf`（46 頁）：附加預期的菲利浦曲線、三次歷史變異、工資指數化、名目工資向下僵固性、盧卡斯批判與沃克反通膨
  3. `raw/Chap-9.pdf`（28 頁）：IS-LM-PC 中期模型、自然實質利率 $r_n$、中期貨幣中立性、1929 大蕭條通縮螺旋、石油危機停滯性通膨
  4. `raw/Chap-10.pdf`（50 頁）：長期經濟成長事實、美俄購買力平價（PPP）、伊斯特林悖論 vs. 131 國快樂實證、馬爾薩斯陷阱、亞洲四小龍收斂、索洛總體生產函數
  5. `raw/Chap-11.pdf`（61 頁）：索洛成長模型穩態 $K^*/N$、二戰後法國重建奇蹟、儲蓄率三大定理、資本黃金法則 $s_G = \alpha$、「明天存更多」與人力資本 $H$
- **Gate 1 前置算式驗算與手寫勘誤攔截（共攔截 3 處投影片印刷錯誤 + 2 處跨章節演進）**：
  1. **`Chap-8.pdf` p.21 不等號印反**：原投影片誤印 $u_t < u_n \implies \pi_t < \pi_{t-1}$；依公式 $\pi_t - \pi_{t-1} = -\alpha(u_t - u_n)$ 與課堂紅筆手寫勘誤修正為 $u_t < u_n \implies \pi_t > \pi_{t-1}$。
  2. **`Chap-9.pdf` p.6 預期參數印錯**：原投影片誤印 `If \theta = 1 (anchored expected inflation)`；依 $\pi^e = (1-\theta)\bar{\pi} + \theta\pi_{-1}$ 與課堂手寫勘誤修正為 **$\theta = 0$**。
  3. **`Chap-11.pdf` p.61 附錄穩態資本公式重大筆誤**：原投影片誤將 Cobb-Douglas 穩態人均資本印成 $K^*/N = (s/\delta)^{\frac{\alpha}{1-\alpha}}$（混淆了 $Y^*/N$ 與 $K^*/N$，並與 p.40–41 數值模擬直接矛盾）；經獨立驗算與核對 p.18, 27, 50 教授手寫板書，修正為 $K^*/N = (s/\delta)^{\frac{1}{1-\alpha}}$、$Y^*/N = (s/\delta)^{\frac{\alpha}{1-\alpha}}$。
  4. **跨章節演進標記**：於 `okuns-law-and-phillips-curve.md` 補充 Ch.9 勞動囤積（Labor Hoarding）與怯志工作者機制，並建立 `saving-short-run-paradox-vs-long-run-growth.md` 串聯 Ch.3 節儉矛盾、Ch.9 中期降息轉投資與 Ch.11 索洛長期資本累積。
- **新建與更新 Wiki 頁面（共新增 11 頁、更新 3 頁，總計 29 個 Wiki 節點）**：
  - 新增來源頁：`source-blanchard-chap-7.md` ～ `source-blanchard-chap-11.md`（5 頁）
  - 新增概念頁：`labor-market-wage-and-price-setting.md`、`expectations-augmented-phillips-curve.md`、`is-lm-pc-medium-run-and-supply-shocks.md`、`economic-growth-ppp-and-happiness.md`、`solow-growth-model-and-golden-rule.md`（5 頁）
  - 新增比較頁：`saving-short-run-paradox-vs-long-run-growth.md`（1 頁）
  - 更新頁面：`okuns-law-and-phillips-curve.md`、`overview.md`、`index.md`

---

## [2026-11-16] outline | 產出第 7–11 章教學簡報結構化大綱 (`slide-outline-ch7-11.md`) (等待 Gate 2 確認)
- **目標受眾與風格**：針對零基礎大學生與一般大眾，全繁體中文標題與生活化案例（亨利·福特加薪降離職率、減薪心理抗拒、1929 通縮死亡螺旋、大麥克與美俄購買力平價、對數所得與快樂、辦公室買電腦的邊際遞減、存錢的黃金法則与「明天存更多」），共規劃 **16 頁**。


---

## [2026-11-16] slides | 通過 Gate 2 大綱檢查（加入短期 vs. 中期對比），編譯產出 18 頁教學簡報 (`slides-ch7-11.html`) (Gate 3)
- **使用者回饋與大綱更新**：
  - 依使用者要求加入「短期 vs. 中期對比」，於 `wiki/comparisons/` 新建 `short-run-vs-medium-run-macro.md`，並將 `slide-outline-ch7-11.md` 擴充為 18 頁（新增第 2 頁「菜單不改價 vs. 薪水物價全面調整」、第 10 頁「降息與減支在短期與中期的相反結局」，並於第 18 頁完成「短、中、長期三維度總貫通」）。
- **產出檔案**：`slides-ch7-11.html`（共 18 頁米色極簡教學簡報，內建第 11 頁「1929 通縮死亡螺旋計算機」、第 17 頁「索洛黃金法則儲蓄率模擬器」、右上角 **「✎ 編輯文字模式（`contenteditable`）」** 與 **「💾 儲存下載 HTML」** 功能）。
- **Gate 3 最終檢查**：
  1. 第 1～18 頁投影片底部皆明確對應 `[[Wiki 節點]]` 與 `Chap-7.pdf` ～ `Chap-11.pdf` 原始頁碼。
  2. 全繁體中文標題與生活化案例，無冗餘英文標籤。
