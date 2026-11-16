---
title: "Blanchard Ch.8：菲利浦曲線、自然失業率與通貨膨脹 (The Phillips Curve, the Natural Rate of Unemployment, and Inflation)"
category: source
source_path: "../../raw/Chap-8.pdf"
source_date: 2026-11-16
author: "Olivier Blanchard (Macroeconomics, 8th Edition)"
tags:
  - source
  - macroeconomics
  - phillips-curve
  - inflation
  - natural-rate-of-unemployment
  - lucas-critique
created: 2026-11-16
updated: 2026-11-16
source_count: 1
status: active
---

# Blanchard Ch.8：菲利浦曲線、自然失業率與通貨膨脹

- **原始檔案**：[Chap-8.pdf](../../raw/Chap-8.pdf)（共 46 頁，含課堂教授手寫推導與勘誤註記）
- **核心主題**：由第 7 章勞動市場 `WS-PS` 模型推導出**附加預期的菲利浦曲線（Expectations-Augmented Phillips Curve）**，探討美國菲利浦曲線在 1960 年代、1970–1995 年代與 1996 年後的三大結構變異（Mutations），定義自然失業率（Natural Rate of Unemployment, $u_n$）及其跨國與跨期變動原因，並分析工資指數化（Wage Indexation）、名目工資向下僵固性（Downward Nominal Wage Rigidity）與反通膨政策可信度（Lucas Critique vs. Volcker Disinflation）。

---

## 1. Gate 1 前置驗算與手寫勘誤檢查紀錄

> [!WARNING] Gate 1 算式與投影片印刷筆誤修正 (`Chap-8.pdf` p.21)
> - **原始投影片誤印（Slide 21）**：在推導自然失業率與加速型菲利浦曲線 $\pi_t - \pi_{t-1} = -\alpha(u_t - u_n)$ 時，投影片第 21 頁第 2 點誤印為：
>   $$u_t < u_n \implies \pi_t < \pi_{t-1}$$
>   $$u_t > u_n \implies \pi_t > \pi_{t-1}$$
> - **Gate 1 驗算與課堂手寫勘誤**：因為 $\alpha > 0$，當實際失業率低於自然失業率（$u_t < u_n$，即 $u_t - u_n < 0$）時，$-\alpha(u_t - u_n) > 0$，通膨率必然**上升**（$\pi_t > \pi_{t-1}$）。課堂手寫筆記已用紅筆將第一行的 `<` 改為 `>`，第二行的 `>` 改為 `<`：
>   $$u_t < u_n \implies \pi_t > \pi_{t-1} \quad (\text{勞動市場過熱，通膨加速})$$
>   $$u_t > u_n \implies \pi_t < \pi_{t-1} \quad (\text{勞動市場冷卻，通膨減速})$$

---

## 2. 核心公式與模型推導

1. **從 WS-PS 模型到價格水準方程式（Slides 4–7）**：
   - 工資設定（WS）：$W = P^e F(u, z)$，線性化設定 $F(u, z) = 1 - \alpha u + z$。
   - 價格設定（PS）：$P = (1 + m)W$。
   - 合併代入得：$P = P^e (1 + m)(1 - \alpha u + z)$。
2. **附加預期的菲利浦曲線（Expectations-Augmented Phillips Curve，Slides 7, 46）**：
   - 將上式對數近似（$\ln(1+x) \approx x$）並減去前期物價對數 $\ln P_{t-1}$，可得通膨率與預期通膨率、加成 $m$、制度變數 $z$ 及失業率 $u_t$ 的關係：
     $$\pi_t = \pi_t^e + (m + z) - \alpha u_t$$
   - **工資—物價螺旋（Wage-Price Spiral，Slide 8）**：低失業率 $u_t \downarrow \implies$ 名目工資 $W_t \uparrow \implies$ 廠商調漲價格 $P_t \uparrow \implies$ 勞工要求更高工資 $W_{t+1} \uparrow \implies$ 物價持續上漲。
3. **通膨預期形成機制（Slide 12）**：
   $$\pi_t^e = (1 - \theta)\bar{\pi} + \theta \pi_{t-1}$$
   - $\theta$ 代表前期通膨率對本期通膨預期的影響權重（預期脫錨程度）。
   - 代回菲利浦曲線：
     $$\pi_t = (1 - \theta)\bar{\pi} + \theta \pi_{t-1} + (m + z) - \alpha u_t$$

---

## 3. 菲利浦曲線的三次歷史變異（The Mutations of the Phillips Curve，Slides 9–22）

| 歷史時期 | 預期參數 $\theta$ | 菲利浦曲線型態與美國實證迴歸式 | 經濟直覺與制度背景 |
| :--- | :--- | :--- | :--- |
| **1. 早期菲利浦曲線（1961–1969）** | $\theta = 0$<br>（通膨預期錨定於 $\bar{\pi} \approx 0$） | $$\pi_t = \bar{\pi} + (m + z) - \alpha u_t$$<br>（失業率與「通膨率水準」呈穩定負相關） | 1960 年代通膨正負交替、平均接近零，工資談判假設明年物價穩定。政府誤以為可用高通膨永久換取低失業。 |
| **2. 加速型菲利浦曲線（1970–1995）** | $\theta = 1$<br>（預期脫錨，$\pi_t^e = \pi_{t-1}$） | $$\pi_t - \pi_{t-1} = (m + z) - \alpha u_t$$<br>美國 1970–1995 迴歸（Slide 17）：<br>$$\pi_t - \pi_{t-1} = 7.4\% - 1.2 u_t \implies u_n \approx 6.2\%$$ | 1970 年代兩次石油危機加上 1960 年代末過熱，使通膨持續為正。勞資雙方改以「去年通膨率」作為預期，原菲利浦曲線消失，轉為失業率與「通膨率變動量」呈負相關（NAIRU）。 |
| **3. 預期再錨定時期（1996–2018）** | $\theta = 0$<br>（央行通膨目標制錨定於 $\bar{\pi}^e = 2\%$） | $$\pi_t = \bar{\pi}^e + (m + z) - \alpha u_t$$<br>美國 1996–2018 迴歸（Slide 19）：<br>$$\pi_t = 2.8\% - 0.16 u_t \implies u_n = 5.0\%$$ | 1990 年代中葉起聯準會成功將通膨預期錨定在 $2\%$，菲利浦曲線重新回到「失業率與通膨水準」的關係，且斜率大幅平坦化（$\alpha$ 由 $1.2$ 降至 $0.16$）。 |

---

## 4. 自然失業率（Natural Rate of Unemployment, $u_n$）與結構演變

- **定義與推導（Slide 20）**：使實際通膨等於預期通膨（$\pi_t = \pi_t^e$）的失業率水準：
  $$0 = (m + z) - \alpha u_n \implies u_n = \frac{m + z}{\alpha}$$
  將 $m + z = \alpha u_n$ 代回，可得標準形式：
  $$\pi_t - \pi_t^e = -\alpha(u_t - u_n)$$
- **為什麼美國自然失業率從 1980 年代的 6%–7% 降至 4%–5%？（Slides 41–45）**：
  1. **全球化與外國競爭加劇**：壓低廠商定價加成 $m$，並削弱工會與勞工議價能力 $z$。
  2. **勞動市場媒合效率提升**：美國臨時派遣機構（Temporary help agencies）佔總就業比例由 1980 年不到 $0.5\%$ 上升至超過 $2\%$，加上網路求職平台普及，降低了摩擦性失業。
  3. **人口高齡化（Aging Population）**：16–24 歲年輕勞工頻繁換工作、失業率高；隨著嬰兒潮世代步入中年，16–24 歲勞動人口佔比由 1980 年的 $24\%$ 降至 2018 年的 $13\%$，拉低整體自然失業率。
  4. **監禁率上升與失能保險（Disability Insurance）擴張**：部分原本容易失業的群體退出勞動力統計。

---

## 5. 三大進階機制與政策爭論（Slides 23–40）

1. **工資指數化（Wage Indexation, $\lambda$，Slides 23–25）**：
   - 若比例為 $\lambda$ 的勞動契約會隨「當期實際通膨 $\pi_t$」自動調薪，而 $1-\lambda$ 隨預期通膨 $\pi_t^e$ 調薪：
     $$\pi_t = \left[\lambda \pi_t + (1 - \lambda)\pi_t^e\right] - \alpha(u_t - u_n)$$
   - 當 $\pi_t^e = \pi_{t-1}$ 時，移項整理得：
     $$\pi_t - \pi_{t-1} = -\frac{\alpha}{1 - \lambda}(u_t - u_n)$$
   - **風險**：工資指數化乘數 $\frac{1}{1-\lambda} > 1$ 會大幅放大失業率缺口對通膨的衝擊；當 $\lambda \to 1$ 時，微小的失業變動就會引發劇烈的通膨暴衝。
2. **通貨緊縮與名目工資向下僵固性（Deflation & Downward Nominal Wage Rigidity，Slides 26–28, 39–40）**：
   - **大蕭條謎團（1930s Great Depression）**：1930 年代失業率高達 $20\%+$，但物價卻沒有如菲利浦曲線預測般無止境崩跌，1934–1937 年甚至出現正通膨。
   - **原因（貨幣幻覺與名目減薪抗拒）**：勞工願意在通膨 $4\%$ 時接受名目加薪 $2\%$（實質減薪 $2\%$），但極度抗拒在通膨 $0\%$ 時直接被「名目扣薪 $2\%$」（Slide 40 葡萄牙 1984 高通膨期 vs. 2012 低通膨歐債危機期的名目工資變動分佈圖證明，名目工資變動在 $0\%$ 處有極高的尖峰堆積）。因此，在零通膨或通縮環境下，菲利浦曲線會變平甚至失效。
3. **反通膨（Disinflation）、政策可信度與盧卡斯批判（Lucas Critique，Slides 30–38）**：
   - **1979 年美國高通膨困境**：通膨高達 $13.3\%$，聯準會主席 Paul Volcker 決心壓低通膨。
   - **傳統派（Traditionalists）**：認為通膨預期具僵固性（$\pi_t - \pi_{t-1} = -0.55(u_t - 6\%)$），若要把通膨從 $10\%$ 降到 $4\%$（降 $6$ 個百分點），必須付出約 $\frac{6}{0.55} \approx 10.9$ 個「超額失業百分點年（Point-years of excess unemployment）」的慘痛衰退代價。
   - **盧卡斯批判（Robert Lucas & Thomas Sargent）**：認為傳統計量模型忽略了「政策改變會直接改變大眾預期」。只要央行展現絕對可信度（Credibility），人們立即下修預期 $\pi_t^e$，反通膨根本不需要經歷高失業（Sargent 舉一戰後奧地利、德國惡性通膨終結為例）。
   - **歷史實證（Table 8-1，1979–1985 Volcker 反通膨）**：Volcker 將 3 個月國庫券利率拉升至 $15\%$（1981 年 8 月），卻因 1980 年中一度放鬆銀根而折損可信度；最終美國在 1980–1982 年爆發嚴重雙底衰退，1982 年底失業率飆至 $10.8\%$，1980–1985 年累計超額失業高達 **$12.7$ 個百分點年**，與傳統派預測高度吻合。

---

## 6. 關聯 Wiki 頁面

- `[[expectations-augmented-phillips-curve|附加預期的菲利浦曲線、自然失業率與通膨動態]]`
- `[[okuns-law-and-phillips-curve|奧肯定律與菲利浦曲線 (Okun's Law & Phillips Curve)]]`
- `[[labor-market-wage-and-price-setting|勞動市場：工資與價格設定模型 (WS-PS Model)]]`
- `[[is-lm-pc-medium-run-and-supply-shocks|IS-LM-PC 中期模型、貨幣中立性與供給衝擊]]`
