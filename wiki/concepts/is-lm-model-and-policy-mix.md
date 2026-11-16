---
title: "IS-LM 模型與財政貨幣政策搭配 (The IS-LM Model & Policy Mix)"
category: concept
tags:
  - macroeconomics
  - is-lm
  - fiscal-policy
  - monetary-policy
  - crowding-out
created: 2026-11-16
updated: 2026-11-16
source_count: 3
status: active
---

# IS-LM 模型與財政貨幣政策搭配 (The IS-LM Model & Policy Mix)

由 John Hicks（1937）與 Alvin Hansen 將凱因斯理論形式化而成的 **`IS-LM` 模型**，是結合**商品市場（Goods Market, `IS`）**與**金融市場（Financial Markets, `LM`）**，用以分析**短期（物價水準固定 $P = \bar{P}$）**產出與利率決定的核心框架（[[source-blanchard-chap-5|Blanchard Ch.5]]）。

---

## 1. IS 曲線：納入內生投資的商品市場均衡

### 1.1 內生投資函數與 IS 方程式
放棄第 3 章投資外生固定的假設，企業投資（$I$）取決於兩大變數：
$$I = I(Y, i), \quad \frac{\partial I}{\partial Y} > 0 \ (\text{加速效果}), \quad \frac{\partial I}{\partial i} < 0 \ (\text{借貸資金成本})$$
代入商品市場均衡條件 $Y = Z$，可得 **`IS` 關係式（Investment = Saving）**：
$$Y = C(Y - T) + I(Y, i) + G$$
- **推導邏輯**：當利率上升（$i \uparrow$）$\implies$ 投資減少（$I \downarrow$）$\implies$ 總需求線 $ZZ$ 下移，透過乘數效果使均衡產出下降（$Y \downarrow$）。因此在 $(Y, i)$ 平面上，**`IS` 曲線呈負斜率（Downward-sloping）**，線上每一點皆代表商品市場達到均衡。

### 1.2 IS 曲線的斜率決定因素（全微分與投資利率彈性，Slides 11–14）
對 $Y = C(Y - T) + I(Y, i) + G$ 取全微分（令 $dT = dG = 0$，簡化設 $I = I(i)$）：
$$dY = C_{Y_D} dY + I_i di \implies \left.\frac{\partial i}{\partial Y}\right|_{IS} = \frac{1 - C_{Y_D}}{I_i} = \frac{1 - c_1}{\varepsilon_i^I} \cdot \frac{i}{I} < 0$$
（其中 $\varepsilon_i^I = I_i \cdot \frac{i}{I} = \frac{\partial I}{\partial i}\frac{i}{I}$ 為**投資的利率彈性**）。
- **關鍵結論**：
  1. **投資的利率彈性 $|\varepsilon_i^I|$ 愈大**（投資對利率變動愈敏感），`IS` 曲線愈**平坦（Flatter）**。
  2. **邊際消費傾向 $c_1$（乘數）愈大**，`IS` 曲線也愈**平坦**。
  3. **`IS` 愈平坦，央行降息（`LM` 下移）刺激產出 $Y$ 的效果愈強！**

### 1.3 點的移動 vs. 整條 IS 曲線的位移（Slide 10）
- **沿著 `IS` 曲線移動**：由縱軸變數**利率 $i$** 變動所引起的產出 $Y$ 變動。
- **整條 `IS` 曲線左右位移**：在給定利率 $i$ 下，任何改變總需求的非利率因素：
  - **右移（擴張）**：政府支出增加（$G \uparrow$）、減稅（$T \downarrow$）、消費者信心上升（$c_0 \uparrow$）、企業投資信心上升。
  - **左移（緊縮）**：削減支出（$G \downarrow$）、加稅（$T \uparrow$）、消費者恐慌（$c_0 \downarrow$）。

---

## 2. LM 曲線：實質貨幣市場均衡與兩種央行體制

將第 4 章的名目貨幣供需均衡 $M = \$Y \cdot L(i) = P \cdot Y \cdot L(i)$ 同除以物價水準 $P$，得**實質貨幣供需均衡（`LM` 關係式）**：
$$\frac{M}{P} = Y \cdot L(i)$$

根據央行貨幣政策操作體制的不同，`LM` 曲線呈現兩種形態（Slides 15–24 vs. 附錄 Slides 36–45）：

| 比較維度 | 1. 現代利率目標制（水平 `LM` 曲線，正文設定） | 2. 傳統貨幣供給目標制（正斜率 `LM` 曲線，附錄設定） |
| :--- | :--- | :--- |
| **央行操作變數** | 央行直接選擇目標利率 **$i = \bar{i}$**，並自動調整名目貨幣供給 $M$ 以維持該利率。 | 央行固定名目貨幣供給 **$M = \bar{M}$**（在物價 $P$ 固定下，實質貨幣供給 $\frac{\bar{M}}{P}$ 固定）。 |
| **`LM` 曲線斜率** | **水平線（斜率 $= 0$）** | **正斜率（Upward-sloping）**：<br>$$\left.\frac{di}{dY}\right|_{LM} = -\frac{L(i)}{Y \cdot L_i} > 0 \quad (L_i = \frac{\partial L}{\partial i} < 0)$$<br>產出 $Y \uparrow \implies$ 實質貨幣需求右移 $\implies$ 利率 $i \uparrow$。<br>📌 貨幣需求對利率愈敏感（$|L_i|$ 愈大），`LM` 愈平坦；當 $i \to 0$ 陷入**流動性陷阱（$|L_i| \to \infty$）**時，`LM` 左端變為水平。 |
| **曲線如何移動** | 央行降息（$\bar{i} \downarrow$）$\implies$ `LM` 水平下移；<br>央行升息（$\bar{i} \uparrow$）$\implies$ `LM` 水平上移。 | 名目貨幣供給增加（$M \uparrow$）或物價下跌（$P \downarrow$）使 $\frac{M}{P} \uparrow \implies$ `LM` 右移（下移）；反之左移（上移）。 |
| **財政擴張 ($G \uparrow$) 是否有排擠效果？** | **無排擠效果（No crowding-out）**：因央行自動釋出貨幣維持利率 $i = \bar{i}$ 不變，且 $Y \uparrow$ 甚至帶動投資 $I(Y, \bar{i}) \uparrow$！ | **有排擠效果（Crowding-out effect）**：`IS` 右移推升產出 $Y \uparrow$ 與利率 $i \uparrow$，利率上升會抑制民間投資（若 $i \uparrow$ 的負面效果大於 $Y \uparrow$ 的加速效果，則總投資 $I$ 下降）。 |

---

## 3. 實證檢驗：IS-LM 模型的動態傳導與物價僵固性 (Empirical Fit)

根據 Blanchard Ch.5（Slides 28–35，Figure 5-10）針對美國聯準會將聯邦基金利率（`FFR`）調升 `1%` 的計量追蹤研究（含 `60%` 信賴區間）：
1. **實體經濟在短期內明確降溫**：升息後，零售銷售（Retail sales）立即下滑；廠商因銷售減少先被動累積存貨，隨後削減生產（Output 在約 **4～8 個季度**達到最大跌幅約 `-0.6%`），並減少雇傭導致失業率上升。
2. **物價水準在前 6 個季度（1.5 年）幾乎完全不變**：升息後長達 **6 個季度**內，物價水準（Price level）幾乎沒有反應，直到第 6 季之後才開始緩慢下滑。
   - **核心啟示**：實證數據強力支持 `IS-LM` 模型在**短期（約 1.5 年內）假設「物價水準固定」**的合理性；同時也說明一旦進入**中期（Medium run，超過 6 季）**，就必須將物價變動納入模型。

---

## 4. 關聯頁面與來源索引 (References)
- **延伸對比**：[[fiscal-vs-monetary-policy-in-is-lm|短期總體政策對比：財政政策 vs. 貨幣政策與政策組合實證]]
- **相關概念**：[[goods-market-and-multiplier|商品市場均衡、凱因斯消費函數與乘數效果]]、[[money-market-and-monetary-policy|貨幣市場、利率決定與央行政策工具]]、[[extended-is-lm-and-financial-crisis|延伸型 IS-LM 模型、實質利率、風險溢酬與金融危機]]
- **引用來源**：[[source-blanchard-chap-5|Blanchard Macroeconomics Ch.5 - Goods and Financial Markets: The IS-LM Model]]
