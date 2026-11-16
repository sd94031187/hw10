---
title: "IS-LM-PC 中期模型、貨幣中立性與供給衝擊 (The IS-LM-PC Model, Neutrality of Money & Supply Shocks)"
category: concept
tags:
  - macroeconomics
  - is-lm-pc
  - medium-run
  - neutrality-of-money
  - deflation-spiral
  - stagflation
created: 2026-11-16
updated: 2026-11-16
source_count: 2
status: active
---

# IS-LM-PC 中期模型、貨幣中立性與供給衝擊

## 1. 核心架構：將短期需求（IS-LM）與中期供給（PC）合而為一

在 Blanchard 第 9 章中，我們把第 5–6 章代表短期商品與金融市場的 **`IS-LM` 模型**，與第 7–8 章代表勞動市場與通膨動態的 **菲利浦曲線（`PC`）** 結合為完整的 **`IS-LM-PC` 總體模型**：

| 曲線名稱 | 核心方程式 | 經濟意義 |
| :--- | :--- | :--- |
| **IS 曲線（商品市場）** | $$Y = C(Y - T) + I(Y, r + x) + G$$ | 實質政策利率 $r$ 越低（或財政支出 $G$ 越高、風險溢酬 $x$ 越低），總需求與短期產出 $Y$ 越高。 |
| **LM 曲線（央行的利率法則）** | $$r = \bar{r}$$ | 現代央行直接設定實質政策利率 $r$ 來調控總需求。 |
| **PC 曲線（以產出缺口表示的菲利浦曲線）** | $$\pi - \pi^e = \frac{\alpha}{L}(Y - Y_n)$$ | 因為就業 $N = L(1-u) = Y$，故產出缺口 $Y - Y_n = -L(u - u_n)$。當實際產出高於潛在產出（$Y > Y_n$），通膨高於預期（$\pi > \pi^e$）。 |

> [!WARNING] Gate 1 參數印刷筆誤提醒 (`Chap-9.pdf` p.6)
> 原始投影片第 6 頁在推導錨定預期下的 PC 曲線 $\pi - \bar{\pi} = \frac{\alpha}{L}(Y - Y_n)$ 時，將條件誤印為 `If \theta = 1 (anchored expected inflation)`。經 Gate 1 驗算與課堂手寫修正：在 $\pi^e = (1-\theta)\bar{\pi} + \theta \pi_{-1}$ 中，**預期錨定於目標 $\bar{\pi}$ 對應的是 $\theta = 0$**（$\theta = 1$ 為脫錨適應性預期 $\pi^e = \pi_{-1}$）。

---

## 2. 從短期收斂到中期：自然實質利率（$r_n$）與貨幣中立性

### 2.1 中期均衡與自然實質利率（Natural Rate of Interest, $r_n$）
- 若短期經濟過熱（$Y > Y_n, u < u_n$），通膨會超過目標或不斷加速（$\pi > \pi^e$）。
- 央行為了平抑通膨，會逐步調升實質政策利率 $r \uparrow \implies$ 企業投資減少、產出沿 `IS` 曲線下滑 $Y \downarrow$，直到**產出剛好回到潛在產出（$Y = Y_n$）、失業率回到自然失業率（$u = u_n$）、通膨穩定在目標（$\pi = \bar{\pi}$）**。
- 此時對應的實質利率稱為**自然實質利率（$r_n$，又稱 Wicksellian Rate 或中性利率 $r^*$）**。在沒有供給衝擊時，穩定產出同時就能穩定通膨，總經學界稱之為**「神聖巧合（Divine Coincidence）」**。

### 2.2 中期貨幣中立性（Neutrality of Money in the Medium Run）
在中期，貨幣政策能改變實質 GDP 嗎？**完全不能！**
- **實質變數由供給面決定**：中期產出永遠收斂回 $Y_n$，失業率收斂回 $u_n$，實質利率收斂回 $r_n$。
- **名目變數由貨幣決定**：在中期，名目貨幣供給成長率 $g_M$ 只會 1 對 1 轉化為通貨膨脹率（$\pi = g_M$），並透過費雪效應把名目利率墊高為 $i = r_n + g_M$。這就是著名的**「貨幣中立性」**（Milton Friedman：「通貨膨脹在任何時間、任何地點都是一種貨幣現象」）。

---

## 3. 當自動收斂失靈：零利率下限與通縮螺旋（Deflation Spiral）

如果中期看似會自動回到 $Y_n$，為什麼 1929 年美國大蕭條會崩潰長達 4 年、失業率飆到 $24.9\%$？
- **致命機制（零利率下限 ZLB + 通縮陷阱）**：
  1. 股市崩盤與銀行倒閉使 `IS` 大幅左移，產出遠低於潛在產出（$Y \ll Y_n$），自然實質利率跌至負值（$r_n < 0$）。
  2. 央行把名目利率降到接近 $0\%$（受制於零利率下限 $i \ge 0$）後無法再降。
  3. 但因為 $Y < Y_n$，根據 `PC` 曲線，經濟陷入**通貨緊縮（$\pi < 0 \implies \pi^e < 0$）**！
  4. 根據實質利率公式 $r = i - \pi^e = 0 - \pi^e > 0$，**通縮越嚴重，實質借款利率 $r$ 反而自動飆得越高**！
  5. 實質利率飆高進一步扼殺投資與消費（$Y$ 跌得更深）$\implies$ 引發更嚴重的通縮（$\pi$ 更負）$\implies$ 形成無法自拔的**「通縮死亡螺旋（Deflation Spiral）」**。
- **1929–1933 年大蕭條實證數據（`[[source-blanchard-chap-9]]`）**：1931–1932 年美國名目利率雖在 $3.1\%–4.0\%$，但因物價暴跌 $-9.2\%$ 與 $-10.8\%$，**事後實質利率竟高達 $12.3\%$ 與 $14.8\%$**！

---

## 4. 供給面衝擊：石油危機與停滯性通膨（Stagflation）

當 1970 年代 OPEC 石油禁運導致油價暴漲時，為何會同時出現「經濟衰退」與「高通膨」？
1. **潛在產出萎縮**：油價屬於非勞動生產成本，油價大漲等同於廠商對工資的加成比例 $m$ 大幅上升 $\implies$ 勞動市場 `PS` 曲線下移 $\implies$ **自然失業率上升（$u_n \uparrow$）、潛在產出下降（$Y_n \to Y_n' < Y_n$）**。
2. **PC 曲線向上移動**：由於潛在產出變小了，原本正常的產出水準現在變成了「過熱（$Y > Y_n'$）」，物價開始加速上漲（$\pi \uparrow$）。
3. **央行的兩難與停滯性通膨（Stagflation）**：央行被迫升息（將實質利率由 $r_n$ 調高至 $r_n'$）來壓抑通膨，最終經濟在伴隨高通膨的過程中，產出萎縮至更低的 $Y_n'$。

---

## 5. 關聯頁面與來源

- **原始教材來源**：
  - `[[source-blanchard-chap-9|Blanchard Ch.9：從短期到中期：IS-LM-PC 模型]]`
- **概念與延伸連結**：
  - `[[extended-is-lm-and-financial-crisis|擴充版 IS-LM 模型：實質利率、風險溢酬與零利率下限]]`
  - `[[expectations-augmented-phillips-curve|附加預期的菲利浦曲線、自然失業率與通膨動態]]`
  - `[[short-run-vs-medium-run-macro|總體經濟的短期與中期對決：需求驅動 vs. 供給約束]]`
