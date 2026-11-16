---
title: "Blanchard Ch.9：從短期到中期：IS-LM-PC 模型 (From the Short to the Medium Run: The IS-LM-PC Model)"
category: source
source_path: "../../raw/Chap-9.pdf"
source_date: 2026-11-16
author: "Olivier Blanchard (Macroeconomics, 8th Edition)"
tags:
  - source
  - macroeconomics
  - is-lm-pc
  - medium-run
  - deflation-spiral
  - stagflation
created: 2026-11-16
updated: 2026-11-16
source_count: 1
status: active
---

# Blanchard Ch.9：從短期到中期：IS-LM-PC 模型

- **原始檔案**：[Chap-9.pdf](../../raw/Chap-9.pdf)（共 28 頁，含課堂手寫修正與圖解標註）
- **核心主題**：將短期商品與金融市場均衡（`IS-LM` 模型）與中期勞動市場及通膨動態（`PC` 菲利浦曲線）整合為 **`IS-LM-PC` 模型**，建立以「產出缺口（Output Gap, $Y - Y_n$）」表示的菲利浦曲線，分析短期到中期的動態收斂、自然實質利率（$r_n$）、貨幣中立性（Neutrality of Money），並探討三大複雜情境：**零利率下限與通縮螺旋（1929–1933 大蕭條）**、**財政整頓（Fiscal Consolidation）**與**石油危機供給衝擊（Stagflation 停滯性通膨）**。

---

## 1. Gate 1 前置驗算與手寫勘誤檢查紀錄

> [!WARNING] Gate 1 參數印刷筆誤修正 (`Chap-9.pdf` p.6)
> - **原始投影片誤印（Slide 6）**：在通膨預期公式 $\pi_t^e = (1 - \theta)\bar{\pi} + \theta \pi_{t-1}$ 下方，投影片第 6 頁第 2 點誤印為：
>   `If \theta = 1 (anchored expected inflation): \pi - \bar{\pi} = (\alpha / L)(Y - Y_n)`
> - **Gate 1 驗算與課堂手寫勘誤**：當預期錨定於目標通膨 $\bar{\pi}$（即 $\pi^e = \bar{\pi}$）時，由 $(1-\theta)\bar{\pi} + \theta\pi_{t-1} = \bar{\pi}$ 可知參數必須為 **$\theta = 0$**（而非 $\theta = 1$；$\theta = 1$ 代表預期完全隨上期通膨浮動 $\pi^e = \pi_{t-1}$）。課堂手寫筆記已用紅筆將 `1` 劃掉並改為 **`0`**。

> [!WARNING] 跨章節模型演進：`Chap-2` 與 `Chap-9` 奧肯定律（Okun's Law）參數與解釋深化
> - **第 2 章（[[source-blanchard-chap-2]]）**：以 2000–2018 年美國季資料迴歸得 $\Delta u_t = -0.4 g_{yt} + 0.7\%$（隱含自然成長率約 $1.75\%$）。
> - **第 9 章（Slide 5 & Slides 9–10）**：
>   1. 在理論模型推導中（Slide 5），先假設無生產力成長與勞動參與率變動（$N = L(1-u), Y = N$），推導出產出缺口與失業缺口的 1 對 1 線性換算：$Y - Y_n = -L(u - u_n)$。
>   2. 在實證專欄（Slides 9–10，1960–2018 美國年資料）中，迴歸式為 $u_t - u_{t-1} = -0.4(g_y - 3\%)$，並正式給出係數小於 1（僅 $0.4$）的兩大總經機制：**勞動囤積（Labor Hoarding，企業在景氣波動時調整工時而非按比例裁員/擴編）** 與 **氣餒勞工效應（Discouraged Workers，景氣好轉吸引非勞動力重返求職，抵銷部分失業率降幅）**。

---

## 2. 核心模型：IS-LM-PC 方程式體系（Slides 2–10）

1. **短期商品與金融市場（IS-LM）**：
   - **IS 曲線**：$Y = C(Y - T) + I(Y, r + x) + G$（實質借貸利率 $\hat{r} = r + x$，其中 $r$ 為央行控制的實質政策利率，$x$ 為風險溢酬）。
   - **LM 曲線（利率法則）**：央行直接設定實質政策利率 $r = \bar{r}$。
2. **將菲利浦曲線從「失業缺口」轉換為「產出缺口（Output Gap）」（Slides 4–6）**：
   - 勞動就業量 $N = L(1 - u)$；若生產函數為 $Y = N$，則潛在產出（自然產出）為 $Y_n = L(1 - u_n)$。
   - **產出缺口（Output Gap）**：
     $$Y - Y_n = L(1 - u) - L(1 - u_n) = -L(u - u_n) \implies u - u_n = -\frac{Y - Y_n}{L}$$
   - 代入第 8 章菲利浦曲線 $\pi - \pi^e = -\alpha(u - u_n)$，得到以產出缺口表示的 **PC 曲線**：
     $$\pi - \pi^e = \frac{\alpha}{L}(Y - Y_n)$$
   - **兩種預期情境**：
     - 脫錨預期（$\theta = 1, \pi^e = \pi_{-1}$）：$\pi - \pi_{-1} = \frac{\alpha}{L}(Y - Y_n)$（當 $Y > Y_n$，通膨持續加速）。
     - 錨定預期（$\theta = 0, \pi^e = \bar{\pi}$）：$\pi - \bar{\pi} = \frac{\alpha}{L}(Y - Y_n)$（當 $Y > Y_n$，通膨高於央行目標 $\bar{\pi}$）。

---

## 3. 從短期到中期的動態收斂與貨幣中立性（Slides 11–14）

- **過熱經濟的收斂過程（Slides 11–12）**：
  - 短期若實質利率過低（$r < r_n$），使總產出高於潛在產出（$Y > Y_n$，正產出缺口），則通膨高於預期或持續上升（$\pi > \pi^e$）。
  - 面對通膨壓力，央行逐步調升實質政策利率 $r \uparrow \implies$ 投資與產出沿 IS 曲線下滑 $Y \downarrow$，直到產出回到潛在產出 $Y = Y_n$、通膨穩定於目標 $\pi = \bar{\pi}$。
  - **自然實質利率（Natural / Neutral / Wicksellian Rate of Interest, $r_n$ 或 $r^*$）**：使總需求剛好等於潛在產出 $Y_n$（產出缺口為零、通膨穩定）的實質政策利率。課堂手寫筆記特別標註：**「神聖巧合（Divine Coincidence）」**——在沒有供給面衝擊時，穩定產出缺口（$Y = Y_n$）同時就能穩定通膨（$\pi = \bar{\pi}$）！
- **中期貨幣中立性（Neutrality of Money in the Medium Run，Slides 13–14）**：
  - 在中期均衡下，實質產出固定在 $Y_n$、失業率固定在 $u_n$、實質利率固定在 $r_n$（完全由供給面與實質需求面決定，與貨幣政策無關）。
  - 因為實質貨幣存量 $M/P$ 在中期不變，名目貨幣成長率 $g_M$ 完全轉化為通膨率 $\pi = g_M$。
  - 根據費雪方程式（Fisher Equation），中期名目利率為：
    $$i = r_n + \pi = r_n + g_M$$
  - **結論**：在中期，提高貨幣成長率只會 1 對 1 推升通膨率與名目利率，無法降低失業率或提高產出。

---

## 4. 三大重要政策與衝擊分析（Slides 15–28）

1. **零利率下限與通縮螺旋（Zero Lower Bound & Deflation Spiral，Slides 15–19）**：
   - 當經濟遭遇劇烈負向需求衝擊，使 $Y \ll Y_n$，且自然實質利率跌至負值（$r_n < 0$）時，若央行名目利率受制於零下限（$i = 0$）：
   - 負向產出缺口導致通貨緊縮（$\pi < 0$）$\implies$ 預期通縮（$\pi^e < 0$）$\implies$ 實質利率 $r = i - \pi^e = 0 - \pi^e > 0$ **被迫自動上升** $\implies$ 投資與總需求進一步萎縮 $Y \downarrow \implies$ 通縮更加惡化！這稱為**通縮螺旋（Deflation Spiral / Deflation Trap）**。
   - **歷史鐵證：1929–1933 年美國大蕭條（Slides 17–19 Table 1）**：

| 年份 | 失業率 $u$ (%) | 實質產出成長率 $g_Y$ (%) | 名目利率 $i$ (%) | 通膨率 $\pi$ (%) | 事後實質利率 $r \approx i - \pi$ (%) |
| :---: | :---: | :---: | :---: | :---: | :---: |
| **1929** | 3.2% | -9.8% | 5.3% | 0.0% | 5.3% |
| **1930** | 8.7% | -7.6% | 4.4% | -2.5% | 6.9% |
| **1931** | 15.9% | -14.7% | 3.1% | **-9.2%** | **12.3%** |
| **1932** | 23.6% | -1.8% | 4.0% | **-10.8%** | **14.8%** |
| **1933** | 24.9% | 9.1% | 2.6% | **-5.2%** | **7.8%** |

2. **財政整頓的短期陣痛與中期轉型（Fiscal Consolidation，Slides 20–21）**：
   - 政府加稅 $T \uparrow$ 或減支 $G \downarrow$ 使 `IS` 左移：
     - **短期**：若央行未即時降息，產出跌破 $Y_n$（$Y < Y_n$），通膨下滑。
     - **中期**：央行調降實質利率至新的較低自然利率 $r_n' < r_n$，刺激私人投資 $I \uparrow$ 完全填補政府支出缺口，產出回到 $Y_n$（中期產出不變，但產出結構由政府消費轉向私人投資）。
3. **供給面衝擊：石油危機與停滯性通膨（Supply Shocks & Stagflation，Slides 22–27）**：
   - **衝擊傳導**：原油等非勞動投入成本暴漲 $\implies$ 等同於廠商對工資的加成比例 $m$ 上升 $\implies$ 價格設定曲線 `PS` 下移 $\implies$ **自然失業率上升（$u_n \uparrow$）、潛在產出下降（$Y_n \to Y_n' < Y_n$）**，使 `PC` 曲線上移。
   - **短期停滯性通膨（Stagflation）**：在原利率 $r_n$ 下，實際產出 $Y$ 雖未變，但因潛在產出 $Y_n'$ 已經縮小，形成 $Y > Y_n'$ 的正缺口，推升通膨 $\pi \uparrow$；央行被迫升息至 $r_n' > r_n$ 以壓抑通膨，最終在中期收斂至更低的潛在產出 $Y_n'$。整個過程伴隨**「產出萎縮（Recession）＋高通膨（Inflation）」**的停滯性通膨。
   - **為何 2000 年代油價飆漲沒有重演 1970 年代的大通膨？（Slide 27）**：(1) 勞工議價能力下降，未能要求油價補償加薪（減少 $m$ 的二輪擴散）；(2) 央行通膨目標深植人心，通膨預期牢牢錨定（$\theta \approx 0$）。

---

## 5. 關聯 Wiki 頁面

- `[[is-lm-pc-medium-run-and-supply-shocks|IS-LM-PC 中期模型、貨幣中立性與供給衝擊]]`
- `[[expectations-augmented-phillips-curve|附加預期的菲利浦曲線、自然失業率與通膨動態]]`
- `[[okuns-law-and-phillips-curve|奧肯定律與菲利浦曲線 (Okun's Law & Phillips Curve)]]`
- `[[short-run-vs-medium-run-macro|總體經濟的短期與中期對決：需求驅動 vs. 供給約束]]`
