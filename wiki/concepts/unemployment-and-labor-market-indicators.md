---
title: "失業率與勞動市場指標 (Unemployment & Labor Market Indicators)"
category: concept
tags:
  - macroeconomics
  - unemployment
  - labor-market
  - business-cycle
created: 2026-11-16
updated: 2026-11-16
source_count: 1
status: active
---

# 失業率與勞動市場指標 (Unemployment & Labor Market Indicators)

## 1. 核心定義與基本公式 (Definitions & Core Formulas)

根據 [[source-blanchard-chap-2|Blanchard Macroeconomics Ch.2]] 與台灣行政院主計總處定義，工作年齡民間人口（$P$）可拆解如下：

- **工作年齡民間人口（Working-age Civilian Population, $P$）**：
  $$P = L + D$$
  - **台灣（主計總處）**：年滿 **15 歲以上**之民間人口（排除現役軍人／武裝勞動力與監管人口）。
  - **美國（BLS / CPS 每月訪查 60,000 戶家庭）**：年滿 **16 歲以上**之非機構民間人口（Civilian noninstitutional population）。
- **勞動力（Labor Force, $L$）**：就業人口（$N$ 或 $E$）與失業人口（$U$）之總和：
  $$L = N + U \quad (\text{或 } E + U)$$
  - **就業者（Employed, $N$ 或 $E$）**：目前有工作者（含因休假、生病等暫時缺勤者）。
  - **失業者（Unemployed, $U$）**：目前沒有工作，但**正在積極尋找工作**（美國 CPS 定義為**過去 4 週內**有積極找工作且隨時可上班；以及暫時被解僱等待召回 `On layoff awaiting recall` 者）。
- **非勞動力（Not in the Labor Force, $D$）**：年滿工作年齡但無工作且未尋找工作者（如在學學生、家庭主婦、退休人士，以及**怯志工作者**）。

### 兩大核心比率指標
1. **官方失業率（Official Unemployment Rate, $u$）**：
   $$u = \frac{U}{L} = \frac{U}{E + U} = \frac{L - E}{L}$$
2. **勞動參與率（Labor Force Participation Rate, $LPR$）**：
   $$LPR = \frac{L}{P} = \frac{U + E}{L + D} = \frac{U + E}{U + E + D}$$

---

## 2. 怯志工作者、廣義失業率與勞參率連動 (Discouraged Workers & LPR)

- **怯志工作者（Discouraged Workers，又稱想工作而未找工作者）**：
  - 定義：雖然想工作且隨時可以開始工作，但因景氣低迷、長期找不到工作而**放棄繼續尋找工作**的人。
  - 統計歸類：在官方統計中，一旦放棄找工作，即**不再計入失業者（$U$），而是轉入非勞動力（$D$）**。
- **失業率（$u$）與勞動參與率（$LPR$）的反向連動關係**：
  - 經濟直覺：當景氣惡化、失業率升高時，部分失業者轉為怯志工作者退出勞動力市場，導致勞動參與率下降。
  - **代數推導（課堂手寫筆記，Slide 40）**：
    由 $u = \frac{U}{L} \implies L = \frac{U}{u}$，代入勞參率公式可得：
    $$LPR = \frac{L}{L + D} = \frac{U / u}{(U / u) + D} = \frac{U}{U + uD}$$
    在失業人數 $U$ 與非勞動力 $D$ 固定下，失業率 $u \uparrow$ 與勞參率 $LPR \downarrow$ 呈現結構性反向關係。
- **廣義失業率（Broad Unemployment Rate，台灣補充定義，Slide 41）**：
  $$\text{廣義失業率 (\%)} = \frac{\text{失業者} + \text{想工作而未找工作且隨時可以開始工作者 (怯志工作者)}}{\text{勞動力} + \text{想工作而未找工作且隨時可以開始工作者}} \times 100\%$$

---

## 3. 失業率的分類、自然失業率與景氣循環特性 (Types & Cyclicality)

### 3.1 三種失業類型與潛在產出（Slide 44）
1. **摩擦性失業（Frictional Unemployment）**：勞動者在轉換工作、初次尋職過程中，因資訊不對稱與媒合時間差所產生的短期失業。
2. **結構性失業（Structural Unemployment）**：因產業結構轉型、技術變革或法規制度，導致勞動者技能與職缺需求不匹配所產生的長期失業。
3. **循環性失業（Cyclical Unemployment）**：因總體經濟景氣衰退、總需求不足所導致的失業。
- **自然失業率（Natural Rate of Unemployment, $u_n$）**：
  $$u_n = \text{摩擦性失業率} + \text{結構性失業率}$$
  當實際失業率等於自然失業率（即循環性失業為 0）時的總產出水準，稱為**潛在產出（Potential Output, $Y_f$）**、**充分就業產出（Full-employment Output）**或**自然產出（Natural Output）**。

### 3.2 景氣循環特性（Slide 43）
- **逆循環變數（Counter-cyclical Variable）**：失業率與 GDP 景氣循環呈反向變動（美國 1960–2018 年間失業率介於 `3% ~ 11%`，2008 金融海嘯後於 2010 年逼近 `10%`）。
- **落後指標（Lagging Indicator）**：廠商在景氣復甦初期通常先增加現有員工工時，待確定需求穩健後才擴大招募；景氣轉差初期也因解僱與再招募成本而延後裁員，故失業率變動落後於總產出變動。

---

## 4. 為什麼經濟學家與投資人高度關注失業率？ (Economic & Market Implications)

1. **失業者的福利與心理衝擊（FOCUS: Unemployment and Happiness，Slide 68）**：
   - 根據德國社會經濟追蹤調查（German Socio-Economic Panel, Winkelmann 2014）：
     1. 失業會導致個人幸福感（Life satisfaction index）大幅暴跌；
     2. 幸福感在**實際失業發生前 1~2 年**就已開始下滑（預期裁員焦慮）；
     3. 即使經歷失業後重返職場，幸福感在 **4 年後仍無法完全恢復**至失業前水準（疤痕效應）。
2. **資源配置效率訊號**：高失業率代表經濟體未能有效利用其人力資源，產出低於潛在產出（$Y_t < Y_f$）。
3. **過低失業率的過熱風險（Wage-Inflation Spiral）**：
   - 當失業率過低（$u_t < u_n$）時，經濟體出現**缺工（Labor shortages）**，推升薪資漲幅，進而轉嫁至終端物價，引發**工資-通膨螺旋（Wage-inflation spiral，Slide 42 手寫筆記）**，迫使央行收緊貨幣政策。

---

## 5. 關聯頁面與來源索引 (References)
- **相關概念**：[[gdp-and-national-income-accounting|GDP 與國民所得會計帳]]、[[okuns-law-and-phillips-curve|歐肯法則 (Okun's Law) 與菲利浦曲線 (Phillips Curve)]]、[[inflation-and-price-indexes|通貨膨脹與物價指數]]
- **引用來源**：[[source-blanchard-chap-2|Blanchard Macroeconomics Ch.2 - A Tour of the Book]]
