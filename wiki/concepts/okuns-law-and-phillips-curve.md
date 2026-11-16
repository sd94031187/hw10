---
title: "歐肯法則 (Okun's Law) 與菲利浦曲線 (Phillips Curve)"
category: concept
tags:
  - macroeconomics
  - okuns-law
  - phillips-curve
  - unemployment
  - inflation
  - taiwan-economy
created: 2026-11-16
updated: 2026-11-16
source_count: 3
status: active
---

# 歐肯法則 (Okun's Law) 與菲利浦曲線 (Phillips Curve)

在總體經濟學中，**總產出（Output）**、**失業率（Unemployment Rate）** 與 **通貨膨脹率（Inflation Rate）** 三大核心變數並非獨立運作，而是透過兩條關鍵實證法則緊密連動（[[source-blanchard-chap-2|Blanchard Ch.2, Slides 59–62]]、[[source-blanchard-chap-8|Ch.8]]、[[source-blanchard-chap-9|Ch.9]]）：

$$\text{總產出成長 } (\Delta y_t) \xrightarrow{\text{歐肯法則 (Okun's Law)}} \text{失業率變動 } (\Delta u_t) \xrightarrow{\text{菲利浦曲線 (Phillips Curve)}} \text{通膨率變動 } (\Delta \pi_t)$$

> [!WARNING] 跨章節模型演進：Ch.2 短期實證 vs. Ch.8–Ch.9 理論機制深化 (2026-11-16 更新)
> 1. **歐肯法則係數（$\omega \approx 0.3 \sim 0.4 < 1$）的兩大微觀機制**：在 [[source-blanchard-chap-9|Ch.9 (Slides 9–10)]] 1960–2018 年美國年資料迴歸 $u_t - u_{t-1} = -0.4(g_y - 3\%)$ 中，正式補充為何產出成長高於正常值 `1%` 時，失業率只下降 `0.4%`（而非 1 對 1 下降 `1%`）：
>    - **勞動囤積（Labor Hoarding）**：企業在景氣波動時偏好先調整現有員工加班工時，而非等比例裁員或擴編（因招募與訓練新員工有固定成本）。
>    - **怯志工作者重返職場（Discouraged Workers）**：當景氣好轉、就業增加時，原本退出勞動市場的人重新開始找工作（勞參率上升），抵銷了部分失業率降幅。
> 2. **菲利浦曲線的預期擴充與三次歷史變異**：在 [[source-blanchard-chap-8|Ch.8]] 中，Ch.2 簡介的菲利浦曲線被正式推導為**附加預期的菲利浦曲線** $\pi_t - \pi_t^e = -\alpha(u_t - u_n)$，並隨通膨預期錨定程度 $\theta$ 演變出 1960s（水準關係）、1970–1995（加速型關係）與 1996 後（再錨定且平坦化）三種型態（詳見 [[expectations-augmented-phillips-curve]]）。

---

## 1. 歐肯法則 (Okun's Law)：產出成長與失業率的反向關係

### 1.1 理論公式與定義（Slide 59）
歐肯法則描述**實質 GDP 成長率（或產出缺口變動）**與**失業率變動**之間的負向關係：
$$\Delta u_t = -\omega \Delta y_t + \varepsilon_t$$
- $\Delta u_t = u_t - u_{t-1}$（或相對於自然失業率 $u_n$ 之偏離 $u_t - u_n$）。
- $\Delta y_t$：實質 GDP 成長率（或相對於充分就業產出 $Y_f$ 之缺口 $\frac{Y_t - Y_f}{Y_f}$）。
- $\omega$：**歐肯係數（Okun coefficient）**，衡量產出成長率每增加 `1%` 時，失業率平均下降的百分點。

### 1.2 美國實證數據（2000 Q1 – 2018 Q4，Slides 59–60）
- **回歸斜率（Slope = `-0.3`）**：美國實質 GDP 成長率每提高 `1%`，失業率平均下降約 **`0.3%`**（0.3 個百分點）。
- **橫軸截距（Intercept at $\Delta y = 0.5\%$）**：當季增經濟成長率為 `0.5%` 時，失業率變動 $\Delta u \approx 0$。
  - **經濟意涵**：由於勞動力人口自然成長與勞動生產力持續提升，經濟體必須維持至少一定的正成長率（此圖季資料為 `0.5%`），才能創造足夠的新工作機會以維持失業率不變。

### 1.3 跨國結構對比：為什麼台灣的歐肯係數遠低於美國？（Slide 60 補充與手寫筆記）

| 經濟體 | 歐肯係數 ($\omega$) | 實質 GDP 成長 +1% 對失業率影響 | 產業結構與勞動市場原因解析 |
| :--- | :---: | :---: | :--- |
| **美國 (US)** | **`~0.30`** | 失業率平均下降 `0.30` 個百分點 | 內需服務業占 GDP 比重極高，且勞動市場聘僱與解僱彈性大，景氣擴張時服務業大量吸納就業人口。 |
| **台灣 (TW)** | **`0.10 ~ 0.16`**<br>*(2015 年實證)* | 失業率僅下降 `0.10 ~ 0.16` 個百分點 | **課堂手寫筆記關鍵洞察**：「**TW 技術/資本密集產業，對於 $\downarrow$ 失業率沒 help**」。台灣 GDP 成長高度仰賴半導體、電子零組件與 ICT 硬體出口，此類產業屬高度**資本密集與技術密集**，產值與出口大增主要轉化為資本設備折舊與企業營業盈餘，對整體就業人數的邊際吸納效果較低，因此經濟成長率上升時，失業率下降幅度遠不如美國明顯。 |

---

## 2. 菲利浦曲線 (Phillips Curve)：失業率與通膨的抵換關係

### 2.1 核心機制與實證表現（Slides 61–62）
- **核心關係**：失業率（$u_t$）與通貨膨脹率（或通膨率變動 $\Delta \pi_t$）之間呈現**負斜率（Downward sloping）**關係。
  - 當勞動市場緊俏、**失業率走低**時，企業爭奪勞工推升薪資與生產成本，帶動**通膨率上升**。
  - 當景氣降溫、**失業率走高**時，薪資議價能力減弱，帶動**通膨率下滑**。
- **美國實證（2000 Q4 – 2018 Q4 核心 CPI 通膨率 vs. 失業率）**：
  - 回歸線呈明顯負斜率。
  - 當核心通膨率維持在 `2%` 附近或失業率高於 `5%` 時，通膨壓力明顯受抑。

---

## 3. 關聯頁面與來源索引 (References)
- **相關概念**：[[gdp-and-national-income-accounting|GDP 與國民所得會計帳]]、[[unemployment-and-labor-market-indicators|失業率與勞動市場指標]]、[[inflation-and-price-indexes|通貨膨脹與物價指數]]、[[macroeconomic-time-horizons|總體經濟的時間維度：極短期、短期、中期與長期]]、[[expectations-augmented-phillips-curve|附加預期的菲利浦曲線、自然失業率與通膨動態]]、[[is-lm-pc-medium-run-and-supply-shocks|IS-LM-PC 中期模型、貨幣中立性與供給衝擊]]
- **引用來源**：[[source-blanchard-chap-2|Blanchard Macroeconomics Ch.2 - A Tour of the Book]]、[[source-blanchard-chap-8|Blanchard Ch.8：菲利浦曲線、自然失業率與通貨膨脹]]、[[source-blanchard-chap-9|Blanchard Ch.9：從短期到中期：IS-LM-PC 模型]]
