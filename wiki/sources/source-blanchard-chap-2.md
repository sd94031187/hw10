---
title: "來源摘要：Blanchard Macroeconomics Ch.2 - A Tour of the Book"
category: source
source_path: "../../raw/Chap-2.pdf"
source_date: 2021-01-01
author: "Olivier Blanchard (Pearson, 8th Ed.) 及課程補充講義/手寫筆記"
tags:
  - source
  - macroeconomics
  - gdp
  - unemployment
  - inflation
  - okuns-law
  - phillips-curve
created: 2026-11-16
updated: 2026-11-16
source_count: 1
status: active
---

# 來源摘要：Blanchard Macroeconomics Ch.2 — A Tour of the Book

- **原始檔案**：[Chap-2.pdf](../../raw/Chap-2.pdf)（共 71 頁投影片，含台灣主計總處定義補充與課堂手寫筆記）
- **教材版本**：Olivier Blanchard, *Macroeconomics*, Eighth Edition, Global Edition (Pearson, 2021)
- **消化日期 (Ingested)**：2026-11-16

---

## 1. 核心結論 (Key Takeaways)

1. **總體經濟三大核心變數**：總產出（Output, 以 `GDP` 衡量）、失業率（Unemployment Rate, $u$）與通貨膨脹率（Inflation Rate, $\pi$）是診斷宏觀經濟健康度的三大支柱。
2. **GDP 的三面等價與衡量演進**：
   - 生產面（最終財加總或附加價值加總）、所得面（要素所得加總）、支出面（$Y = C + I + G + X - M$）三者恆等。
   - 為消除物價變動干擾需計算實質 GDP（Real GDP, $Y_t$），但傳統「定基法（Fixed-base）」因相對價格變動（尤其 ICT 產品系統性跌價）會產生嚴重的**替代性偏誤（Substitution Bias）** 且改變基期會改變歷史成長率，故美、台（主計總處）等主要國家已改採 **「連鎖法（Chain-linked Index）」**。
3. **勞動市場與失業率的結構解讀**：
   - 失業率 $u = U / L$ 為**逆循環（Counter-cyclical）**且屬**落後指標（Lagging indicator）**。
   - **怯志工作者（Discouraged workers）** 放棄找工作退出勞動力（計入非勞動力 $D$），使高失業率通常伴隨較低的勞動參與率（$LPR = \frac{U}{U + uD}$）。
4. **物價指數的選擇與偏誤**：
   - `CPI` 採拉氏指數（Laspeyres，固定基期籃子），無法反映消費者替代行為，會**高估通膨與生活成本**；`GDP Deflator` 採畢氏指數（Paasche，當期籃子），會**低估通膨**。
   - 美國聯準會（Fed）自 2012 年 1 月起改以 `PCE`（個人消費支出物價指數）作為首要通膨指標，因其採動態權重（反映替代效果）、涵蓋範圍更廣（含雇主與政府負擔之醫療支出）且可全面回溯修正。
5. **三大宏觀核心法則與跨國結構差異**：
   - **歐肯法則（Okun's Law）**：產出成長率與失業率變動呈負相關（$\Delta u_t = -\omega \Delta y_t + \varepsilon_t$）。美國斜率約 `-0.3`（成長率每高 1%，失業率降 0.3%，且需維持 0.5% 成長率才能保持失業率不變）；**台灣的歐肯係數僅約 `0.1 ~ 0.16`（2015 年）**，反映台灣以資本與技術密集（半導體/ICT）為主的產業結構，GDP 成長對降低失業率的帶動效果明顯較小。
   - **菲利浦曲線（Phillips Curve）**：失業率與通膨變動呈負相關（美國 2000 Q4–2018 Q4 實證顯示，當 $u > 5\%$ 時核心通膨傾向下降；過低的失業率則可能引發缺工與 `wage-inflation spiral` 工資-通膨螺旋）。
6. **總體經濟的時間維度框架（Time Horizons）**：
   - **極短期（Very short run）**：物價水準固定（Constant price level）。
   - **短期（Short run，1–2 年內）**：價格與工資具僵固性（Sticky），產出由**總需求（Demand）**決定（第 3–6 章）。
   - **中期（Medium run，1–2 年以上）**：價格與工資可調整，產出由**總供給（Supply side：資本存量、技術、勞動力規模）**決定（第 7–9 章）。
   - **長期（Long run，數十年以上）**：產出成長取決於**創新與技術進步、儲蓄率、教育系統品質與政府制度品質**（第 10–13 章）。

---

## 2. 關鍵數據、公式與圖表摘錄 (Key Data, Formulas & Tables)

### 2.1 國民所得會計恆等式（含主計總處補充，Slides 4–15）
- **GNI / GNP（國民所得毛額 / 國民生產毛額）**：
  $$\text{GNI} = \text{GDP} + \text{國外要素所得收入淨額 (NFI)}$$
- **NNI（國民所得淨額 / 按市價計算之國民所得）**：
  $$\text{NNI} = \text{GNI} - \text{折舊 (Depreciation)}$$
- **NDP（國內生產淨額）**：
  $$\text{NDP} = \text{GDP} - \text{折舊 (Depreciation)}$$
- **NI（按要素成本計算之國民所得）**：
  $$\text{NI} = \text{NNI} - \text{間接稅淨額（生產及進口稅淨額）} = \text{受僱人員報酬} + \text{營業盈餘（利息+地租+稅後利潤）} + \text{國外要素所得收入淨額}$$
  - 其中：$\text{間接稅淨額} = \text{間接稅} - \text{政府補貼}$。
- **PI（個人所得 Personal Income）**：
  $$\text{PI} = \text{NI} - \text{勞而不獲（營所稅、社會保險、未分配盈餘、企業罰款、政府財產所得）} + \text{不勞而獲（失業保險、社福金、退休年金、補助金、國內外移轉收入淨額、公債利息）}$$
- **國民可支配所得**：按市價計算之國民所得（NNI）$+$ 國外經常移轉收入淨額。

### 2.2 美國實質與名目 GDP 長期實證數據（Slides 19–22, 67）
- **1960–2018 美國 GDP 增長倍數**：名目 GDP（`Nominal GDP`, $\$Y_t$）增長 **38 倍**；實質 GDP（`Real GDP`, $Y_t$，以 2012 年連鎖美元計）增長約 **5.7 倍**，兩者差距來自期間物價水準持續上升。
- **衰退（Recession）的慣例定義**：連續至少 **2 個季度（two consecutive quarters）** 實質 GDP 負成長。
  - **2001 年 Y2K 衰退謎題（Slide 22）**：年資料圖表顯示 2001 全年實質 GDP 為正成長，但因 2001 年前三個季度（Q1–Q3）季增率皆為負值，故仍被認定為溫和衰退。
- **特徵定價法（Hedonic Pricing）與電腦價格（Slide 67）**：
  - 1999 年以來，新款筆電提供的運算服務品質平均每年提升 **20%**，而名目美元售價平均每年下跌 **7%**，因此經品質調整後的實質價格（Quality-adjusted price）平均每年大幅下跌 **$20\% + 7\% = 27\%$**。

### 2.3 連鎖量指數（Chained Volume Index）三期數值範例（Slides 30–34）
假設經濟體生產 A、B、C 三種最終財：

| 商品 | $p_t$ | $p_{t+1}$ | $p_{t+2}$ | $q_t$ | $q_{t+1}$ | $q_{t+2}$ |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| **A** | 7 | 4 | 3 | 10 | 15 | 18 |
| **B** | 10 | 11 | 12 | 12 | 12 | 13 |
| **C** | 3 | 5 | 5 | 20 | 18 | 18 |

- **Step 1（$t \to t+1$，以 $t$ 期為基期）**：
  - $\sum p_t q_t = 7(10) + 10(12) + 3(20) = 70 + 120 + 60 = 250$
  - $\sum p_t q_{t+1} = 7(15) + 10(12) + 3(18) = 105 + 120 + 54 = 279$
  - $g_{t \to t+1} = \frac{279 - 250}{250} = 11.6\%$
- **Step 2（$t+1 \to t+2$，以 $t+1$ 期為基期）**：
  - $\sum p_{t+1} q_{t+1} = 4(15) + 11(12) + 5(18) = 60 + 132 + 90 = 282$（註：投影片第 31 頁手寫修正印刷錯誤 `30` 為 `60`）
  - $\sum p_{t+1} q_{t+2} = 4(18) + 11(13) + 5(18) = 72 + 143 + 90 = 305$
  - $g_{t+1 \to t+2} = \frac{305 - 282}{282} = 8.2\%$
- **Step 3（以 $t$ 期為參考年 Reference Year = 100 推算連鎖量指數與連鎖值 GDP）**：

| 期間 | 名目 GDP ($\$Y$) | 實質 GDP 成長率 | 連鎖量指數 (Chained Volume Index) | 連鎖值實質 GDP (Chained Volume GDP) |
| :---: | :---: | :---: | :---: | :---: |
| **$t$（參考年）** | 250 | - | $100$ | $250$ |
| **$t+1$** | 282 | $11.6\%$ | $100 \times (1 + 11.6\%) = 111.6$ | $250 \times 1.116 = 279$ |
| **$t+2$** | 300 | $8.2\%$ | $111.6 \times (1 + 8.2\%) = 120.7$ | $250 \times 1.207 = 301.7$ |

---

## 3. 觸及與新建的 Wiki 頁面 (Linked Entities & Concepts)

- **新建概念頁面 (`wiki/concepts/`)**：
  - [[gdp-and-national-income-accounting|GDP 與國民所得會計帳]]
  - [[unemployment-and-labor-market-indicators|失業率與勞動市場指標]]
  - [[inflation-and-price-indexes|通貨膨脹與物價指數]]
  - [[okuns-law-and-phillips-curve|歐肯法則 (Okun's Law) 與菲利浦曲線 (Phillips Curve)]]
  - [[macroeconomic-time-horizons|總體經濟的時間維度：極短期、短期、中期與長期]]
- **新建對比頁面 (`wiki/comparisons/`)**：
  - [[fixed-base-vs-chain-linked-gdp|實質 GDP 衡量對比：定基法 (Fixed-Base) vs. 連鎖法 (Chain-Linked)]]
  - [[cpi-vs-pce-vs-gdp-deflator|三大通膨與物價指標對比：CPI vs. PCE vs. GDP Deflator]]
