---
title: "商品市場均衡、凱因斯消費函數與乘數效果 (Goods Market, Multiplier & Paradox of Saving)"
category: concept
tags:
  - macroeconomics
  - goods-market
  - consumption-function
  - multiplier
  - paradox-of-saving
  - fiscal-policy
created: 2026-11-16
updated: 2026-11-16
source_count: 2
status: active
---

# 商品市場均衡、凱因斯消費函數與乘數效果 (Goods Market, Multiplier & Paradox of Saving)

## 1. 短期商品市場的核心循環 (The Short-Run Demand-Production-Income Loop)

在短期（[[macroeconomic-time-horizons|總體經濟時間維度]]）物價水準固定的假設下，經濟活動由以下正向回饋迴圈驅動（[[source-blanchard-chap-3|Blanchard Ch.3]]）：
$$\text{總需求 (Demand, } Z\text{)} \longrightarrow \text{總生產 (Production, } Y\text{)} \equiv \text{總所得 (Income, } Y\text{)} \longrightarrow \text{誘發消費需求 (Demand, } Z\text{)}$$

---

## 2. 凱因斯消費函數與可支配所得 (Keynesian Consumption Function)

民間消費（$C$）主要取決於**可支配所得（Disposable Income, $Y_D \equiv Y - T$）**（其中 $T$ 為稅收減去政府移轉性支付之淨稅收）：
$$C = C(Y_D) = c_0 + c_1 Y_D = c_0 + c_1(Y - T)$$

| 參數 / 指標 | 名稱與公式 | 經濟意涵與實務觀察 |
| :--- | :--- | :--- |
| **$c_0$** | **自發性消費 (Autonomous Consumption)** | 當可支配所得 $Y_D = 0$ 時的基本生存消費；實務上反映在給定當期所得下，由**消費者信心、未來所得預期、財富水準與信貸條件**決定的消費意願。<br>📌 *案例*：2008 年雷曼兄弟破產引發大蕭條恐慌，在當期所得尚未下滑前，美國民眾恐慌性縮減耐久財支出，導致 $c_0$ 大幅下降（消費函數下移）。 |
| **$c_1$** | **邊際消費傾向 (Marginal Propensity to Consume, MPC)**<br>$$c_1 = \frac{\partial C}{\partial Y_D}, \quad 0 < c_1 < 1$$ | 可支配所得每增加 1 美元時，用於增加消費的比例（大於 0 且小於 1，因為人們會將一部分新增所得存起來，體現 `Consumption smoothing` 消費平滑化）。 |
| **$c_1 Y_D$** | **誘發性消費 (Induced Consumption)** | 由當期可支配所得變動所誘發的消費，是產生**乘數效果**的核心引擎。 |
| **$APC$** | **平均消費傾向 (Average Propensity to Consume)**<br>$$APC = \frac{C}{Y_D} = \frac{c_0}{Y_D} + c_1$$ | 圖形上為「原點至消費函數上該點連線之斜率」。由於 $c_0 > 0$，恆有 **$APC \ge MPC$**（隨所得提高，$APC$ 遞減並趨近於 $MPC$）。 |
| **$1 - c_1$** | **邊際儲蓄傾向 (Marginal Propensity to Save, MPS)** | 可支配所得每增加 1 美元用於增加私人儲蓄的比例，恆滿足 **$MPC + MPS = 1$**。 |

---

## 3. 商品市場均衡與三種乘數公式推導 (Equilibrium Output & Multipliers)

在封閉經濟（$X = IM = 0$）中，總需求 $Z \equiv C + I + G$。商品市場均衡要求 **生產等於需求（$Y = Z$）**（若產出大於需求則累積非意願存貨，反之存貨減少）。

### 3.1 基本定額稅模型（$I = \bar{I}$, $T$ 為固定定額稅）
$$Y = c_0 + c_1(Y - T) + \bar{I} + G \implies (1 - c_1)Y = \left[ c_0 + \bar{I} + G - c_1 T \right]$$
$$Y^* = \underbrace{\frac{1}{1 - c_1}}_{\text{乘數 (Multiplier)}} \times \underbrace{\left[ c_0 + \bar{I} + G - c_1 T \right]}_{\text{自發性支出 (Autonomous Spending)}}$$
- **乘數的幾何級數原理**：自發性支出增加 $\$1$ $\rightarrow$ 第一輪產出與所得增加 $\$1$ $\rightarrow$ 第二輪誘發消費增加 $\$c_1$ $\rightarrow$ 第三輪誘發消費增加 $\$c_1^2 \dots$，總產出增幅為無窮等比級數收斂值：
  $$1 + c_1 + c_1^2 + \dots + c_1^n + \dots = \frac{1}{1 - c_1} > 1$$
  （例如當 $c_1 = 0.6$ 時，乘數為 $\frac{1}{1 - 0.6} = 2.5$）。

### 3.2 三種不同財政與稅制設定下的乘數比較（Slides 20–23 課堂補充）

| 乘數類型 | 設定條件 | 乘數公式 ($\frac{\Delta Y^*}{\Delta \text{Shock}}$) | 數值範例 ($c_1 = 0.6, t = 0.2$) | 政策意涵 |
| :--- | :--- | :--- | :--- | :--- |
| **1. 政府支出 / 自發性消費乘數** | 定額稅 $T$，變動 $G$ 或 $c_0$ | $$\frac{1}{1 - c_1}$$ | `2.50` | 直接進入第一輪總需求，乘數最大。 |
| **2. 定額租稅乘數** | 定額稅 $T$，變動 $T$ | $$\frac{-c_1}{1 - c_1}$$ | `-1.50` | 減稅 $\$1$ 第一輪僅使消費增加 $\$c_1$（部分被儲蓄），絕對值小於支出乘數。 |
| **3. 平衡預算乘數 (Balanced Budget Multiplier)** | 定額稅且政府維持預算平衡（$\Delta G = \Delta T$） | $$\frac{1}{1 - c_1} + \frac{-c_1}{1 - c_1} = \frac{1 - c_1}{1 - c_1} = 1$$ | **`1.00`（恆等於 1）** | 政府同時增稅與增加支出各 $\$1$，均衡產出仍會淨增加 $\$1$！ |
| **4. 比例稅支出乘數 (Proportional Tax Multiplier)** | 稅收隨所得變動：$T = T_0 + tY$（$0 < t < 1$） | $$\frac{1}{1 - c_1(1 - t)}$$ | $\frac{1}{1 - 0.6(0.8)} =$ **`1.92`** | 比例所得稅使每一輪誘發所得被抽走 $t$ 比例，削弱乘數效果（充當景氣「**自動穩定器 Automatic Stabilizer**」）。 |

---

## 4. 投資等於儲蓄 ($I = S$) 與節儉矛盾 (The Paradox of Saving)

### 4.1 恆等式推導：為什麼 $Y = Z \iff I = S + (T - G)$？
- **私人儲蓄（Private Saving, $S$）**：可支配所得扣除消費：
  $$S \equiv Y_D - C = Y - T - C = -c_0 + (1 - c_1)(Y - T)$$
- **公共儲蓄（Public Saving）**：政府淨稅收減去政府支出 $= T - G$（$>0$ 為預算盈餘 Budget surplus；$<0$ 為預算赤字 Budget deficit）。
- 由商品市場均衡 $Y = C + I + G$，兩邊同減 $(T + C)$ 可得：
  $$Y - T - C = I + G - T \implies S = I + G - T \implies \mathbf{I = S + (T - G)}$$
  此即著名的 **`IS` 關係（Investment equals Saving，總投資等於私人儲蓄加公共儲蓄）**。

### 4.2 節儉矛盾（Paradox of Saving，Slides 38–40 & [[source-blanchard-chap-5|Ch.5]]）
當消費者因擔心未來景氣而在給定所得下決定「多存錢、少消費」（即自發性消費下降 $c_0 \downarrow$，或自發性儲蓄 $-c_0 \uparrow$）時，對總體經濟的產出與總儲蓄有何影響？

> [!WARNING] 模型假設演進與結論差異：固定投資 vs. 內生加速投資 (2026-11-16 整理)
> - **情況一：基本模型（投資外生固定 $I = \bar{I}$，Ch.3 Slide 38）**
>   - $c_0 \downarrow \implies$ 總需求減少，透過乘數使均衡產出 $Y^* \downarrow$。
>   - 由於 $I = \bar{I}$ 且 $T, G$ 不變，由均衡條件 $S = \bar{I} + G - T$ 可知，**最終均衡私人儲蓄 $S$ 完全不變**！（自發性儲蓄 $-c_0$ 的增加，恰好被所得下降導致的誘發性儲蓄 $(1-c_1)Y$ 減少完全抵銷）。
> - **情況二：納入加速原理的內生投資模型（$I = I(Y)$ 且 $I'(Y) > 0$，Ch.3 Slide 40 補充）**
>   - 當投資取決於產出（**加速效果 The Accelerator Effect**，且儲蓄線斜率大於投資線斜率 $1 - c_1 > I'(Y)$）時：
>   - 自發性儲蓄上升使 $S + T$ 線左移，導致均衡產出 $Y^* \downarrow$，進而拖累企業投資 $I(Y) \downarrow$，最終導致**新的均衡總儲蓄反而低於原本的總儲蓄（$S_1 < S_0$）**——「每個人都想多存錢，結果整體經濟反而存得更少、變得更窮」！

---

## 5. 關聯頁面與來源索引 (References)
- **相關概念**：[[gdp-and-national-income-accounting|GDP 與國民所得會計帳]]、[[is-lm-model-and-policy-mix|IS-LM 模型與財政貨幣政策搭配]]
- **延伸對比**：[[fiscal-vs-monetary-policy-in-is-lm|短期總體政策對比：財政政策 vs. 貨幣政策與政策組合實證]]
- **引用來源**：[[source-blanchard-chap-3|Blanchard Macroeconomics Ch.3 - The Goods Market]]、[[source-blanchard-chap-5|Blanchard Macroeconomics Ch.5 - The IS-LM Model]]
