---
title: "三大通膨與物價指標對比：CPI vs. PCE vs. GDP Deflator"
category: comparison
tags:
  - comparison
  - inflation
  - cpi
  - pce
  - gdp-deflator
  - federal-reserve
created: 2026-11-16
updated: 2026-11-16
source_count: 1
status: active
---

# 三大通膨與物價指標對比：CPI vs. PCE vs. GDP Deflator

## 1. 核心結論與勝負手 (Executive Verdict)

- **一句話總結**：
  - **GDP 平減指數（GDP Deflator）** 衡量「一國**國內生產**所有最終財（含企業投資、政府支出與出口，不含進口）」的價格變動；
  - **消費者物價指數（CPI）** 與 **個人消費支出物價指數（PCE）** 則聚焦於「**消費者購買**（含進口消費品）」的生活成本（Cost of living）。
  - 在 `CPI` 與 `PCE` 之間，由於 **CPI 採用固定權重的拉氏指數（Laspeyres），無法即時反映消費者替代行為，往往高估生活成本與通膨率**；因此**美國聯準會（Fed）自 2012 年 1 月起正式宣布以 `PCE` 作為貨幣政策的首要通膨衡量指標**。

---

## 2. CPI vs. PCE vs. GDP Deflator 多維度橫向對比表 (Head-to-Head Matrix)

整理自 [[source-blanchard-chap-2|Blanchard Macroeconomics Ch.2（Slides 46–56 教材與補充講義）]]：

| 比較維度 | CPI (消費者物價指數) | PCE (個人消費支出物價指數) | GDP Deflator (GDP 平減指數) |
| :--- | :--- | :--- | :--- |
| **美國發布機構** | **美國勞工統計局 (BLS)** | **美國經濟分析局 (BEA)** | **美國經濟分析局 (BEA)** |
| **資料調查來源 (Data Sources)** | **家庭調查 (Household surveys)**：僅涵蓋全美**都市家庭 (Urban households)**。 | **企業/供應商調查 + GDP 國民所得報告**：涵蓋全美**所有家庭（含非都市）及非營利機構 (Nonprofits)**。 | **國民所得與生產帳戶 (NIPA)**：全體國內生產部門統計。 |
| **商品與服務涵蓋範圍 (Coverage)** | **僅限消費者自掏腰包 (Out-of-pocket) 支出**（約 211 大類消費項目，含進口消費品，不含企業資本財與政府支出）。 | **廣義個人消費支出**：除自付費用外，**包含非由個人直接支付之項目**（如雇主負擔之醫療保險、政府 `Medicare` 與 `Medicaid` 醫療支出）。 | **國內生產之全部最終財 ($C+I+G+X$)**：包含售予企業之投資財、政府採購與出口品，但**完全排除進口品 ($M$)**。 |
| **指數計算公式與權重調整** | **拉氏指數 (Laspeyres Index)**：採用固定基期消費籃子權重（$\frac{\sum P_1 Q_0}{\sum P_0 Q_0}$），**權重較不調整**。 | **連鎖費雪指數 (Chain-type Index)**：**動態調整商品服務權重**，能反映相對價格變化下的消費者替代行為。 | **畢氏指數 (Paasche Index)**（或連鎖平減）：以當期實際產出結構為權重（$\frac{\sum P_1 Q_1}{\sum P_0 Q_1}$）。 |
| **對通膨與波動度之影響** | **高估生活成本與通膨率**；且易受電腦、汽油等價格劇烈波動項目影響，**波動度較高**。 | **平滑極端價格波動 (Smooth out swings)**，能真實反映消費者改變購買模式的實際支出，**波動度較低**。 | 當進口能源或進口商品大漲時，因不含進口品，初期漲幅會低於 CPI。 |
| **歷史資料修正彈性 (Revisions)** | 僅能針對季節性因素調整，且僅限回溯修正過去 5 年內資料。 | 可隨最新完整普查與 GDP 報告進行**更廣泛、長期的歷史資料回溯修正**。 | 隨 GDP 報告定期全面修正。 |

---

## 3. 深度歷史案例與政策解析 (Deep-Dive Analysis)

### 3.1 為什麼 1979–1980 年美國 CPI 漲幅遠高於 GDP Deflator？（Slides 52–53）
- 觀察美國 1960–2018 年的通膨走勢（Figure 2.4），絕大多數時期 `CPI` 通膨率與 `GDP Deflator` 通膨率高度同步。
- **關鍵例外（1974 與 1979–1980 兩次石油危機）**：
  - 在 1979–1980 年第二次石油危機期間，美國 `CPI` 年增率飆破 `13%~14%`，顯著高於 `GDP Deflator`（約 `9%`）。
  - **核心原因**：當時國際原油與**進口商品價格相對於美國國內生產商品價格暴漲**。由於美國消費大量進口原油，進口油價直接推升消費者購買籃子的 `CPI`；但進口品不屬於美國國內生產，在 `GDP`（$C+I+G+X-M$）中已作為減項扣除，故未直接反映在初期的 `GDP Deflator` 上。

### 3.2 為什麼美國聯準會（Fed）自 2012 年 1 月起改用 PCE 取代 CPI？（Slide 56）
聯準會偏好 `PCE`（及扣除食品與能源後的 `Core PCE` 核心個人消費支出物價指數）主要有三大政策考量：
1. **納入消費者替代效果（Substitution Effect）**：當麵包漲價時，民眾會少買麵包、改買其他主食；`PCE` 的支出權重會動態更新以反映新的消費籃子，而 `CPI` 對消費偏好的轉變反應僵固（因而高估生活成本）。
2. **涵蓋範圍更全面（Comprehensive Coverage）**：納入雇主與政府代付的醫療保健等非自付支出，更能反映整體民間消費結構（尤其醫療占美國經濟比重極高）。
3. **資料可全面回溯修正（Extensive Revisions）**：有助於央行更精確地評估長期通膨趨勢與貨幣政策傳導效果。

---

## 4. 關聯頁面與來源索引 (References)
- **相關概念**：[[inflation-and-price-indexes|通貨膨脹與物價指數]]、[[gdp-and-national-income-accounting|GDP 與國民所得會計帳]]
- **延伸對比**：[[fixed-base-vs-chain-linked-gdp|實質 GDP 衡量對比：定基法 (Fixed-Base) vs. 連鎖法 (Chain-Linked)]]
- **引用來源**：[[source-blanchard-chap-2|Blanchard Macroeconomics Ch.2 - A Tour of the Book]]
