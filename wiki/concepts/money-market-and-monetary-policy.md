---
title: "貨幣市場、利率決定與央行政策工具 (Money Market, Central Bank & Liquidity Trap)"
category: concept
tags:
  - macroeconomics
  - money-market
  - monetary-policy
  - central-bank
  - liquidity-trap
  - money-multiplier
created: 2026-11-16
updated: 2026-11-16
source_count: 2
status: active
---

# 貨幣市場、利率決定與央行政策工具 (Money Market, Central Bank & Liquidity Trap)

## 1. 貨幣的功能、存流量區辨與台美貨幣定義 (Functions & Definitions of Money)

### 1.1 貨幣三大功能與存流量語意區辨（[[source-blanchard-chap-4|Blanchard Ch.4, Slides 7–8]]）
- **貨幣三大功能**：交易媒介（Medium of exchange）、計價單位（Unit of account）、價值儲藏（Store of value）。貨幣是全世界流動性最高（Most liquid）的資產，但本身不支付利息。
- **存量（Stock）vs. 流量（Flow）語意陷阱對照表**：

| 存量變數 (Stock Variables：特定時點的累積值) | 流量變數 (Flow Variables：特定期間內的發生額) |
| :--- | :--- |
| **貨幣 (Money)**：可用於支付交易的資產存量（通貨 $+$ 活期/支票存款） | **所得 (Income, $Y$)**：在一定期間內賺取的報酬 |
| **累積儲蓄 / 財富 (Savings / Financial Wealth)**：隨時間累積的總資產減總負債 | **當期儲蓄 (Saving, $S$)**：當期稅後所得未用於消費的部分（$Y_D - C$） |
| **資本存量 (Capital Stock, $K$)** / **金融投資部位 (Financial Investment)** | **實質投資 (Investment, $I$)**：當期購買新資本財（廠房、設備、新屋）之支出 |

### 1.2 台灣中央銀行 vs. 美國聯準會之貨幣總計數定義（Slides 6, 24, 46）

| 貨幣層級 | 組成定義 | 流動性與金融市場意義 |
| :--- | :--- | :--- |
| **台灣 `M1A`** | $\text{通貨淨額 (Currency)} + \text{支票存款} + \text{活期存款}$（對應美國傳統 `M1`） | 交易媒介屬性最強、**流動性最高**。 |
| **台灣 `M1B`** | $\text{M1A} + \text{活期儲蓄存款（個人或非營利法人持有）}$ | 台灣散戶與法人資金停泊處，實務上常作為**台股資金動能指標**。 |
| **台灣 `M2`** | $\text{M1B} + \text{準貨幣（Quasi-money：定期存款、定期儲蓄存款、外匯存款、郵政儲金、附買回交易餘額 RP、外國人新台幣存款、貨幣市場共同基金 MMMF）}$ | 廣義貨幣供給，流動性較 `M1B` 低，為央行監測長期物價與信用擴張的核心指標。 |

---

## 2. 貨幣需求、公開市場操作與債券定價 (Money Demand & OMO)

### 2.1 貨幣需求函數（Slides 8–10）
$$M^d = \$Y \cdot L(i), \quad L'(i) < 0$$
- **交易動機（$\$Y$）**：名目所得增加 $\implies$ 交易規模擴大 $\implies$ 在給定利率下，貨幣需求曲線 **$M^d$ 右移**。
- **機會成本（$i$）**：短期債券名目利率 $i$ 上升 $\implies$ 持有無息貨幣的機會成本提高，人們將財富轉入債券（或透過開放式貨幣市場共同基金 `MMMF` 間接持有短期債券）$\implies$ 沿著 $M^d$ 曲線左上移動（貨幣需求量減少）。

### 2.2 貼現債券價格與利率的反向關係（Slides 14, 18–20）
假設一年期國庫券（Treasury bill, `T-bill`，期限 $<1$ 年；另有 $2\sim10$ 年期 `T-notes` 及 $30$ 年期 `T-bonds`）承諾一年後償還面額 $\$100$，今日市場價格為 $\$P_B$，則其隱含名目利率（殖利率）為：
$$i = \frac{\$100 - \$P_B}{\$P_B} \iff \$P_B = \frac{\$100}{1 + i}$$
> **核心鐵律**：**債券價格（$\$P_B$）與利率（$i$）呈嚴格反向關係**。

### 2.3 央行的公開市場操作（Open Market Operations, OMO）
- **擴張性公開市場操作（Expansionary OMO）**：央行在債券市場**買入債券**並釋出貨幣 $\implies$ 債券需求增加推升債券價格 $\$P_B \uparrow$ $\implies$ **市場利率 $i \downarrow$**（貨幣供給 $M^s$ 右移）。
- **緊縮性公開市場操作（Contractionary OMO）**：央行在債券市場**賣出債券**並收回貨幣 $\implies$ 債券供給增加壓低債券價格 $\$P_B \downarrow$ $\implies$ **市場利率 $i \uparrow$**（貨幣供給 $M^s$ 左移）。

---

## 3. 銀行資產負債表、強力貨幣與貨幣乘數 (Monetary Base & Money Multiplier)

當納入商業銀行（Financial intermediaries）吸收支票存款（Checkable deposits, $D$）並保留比例 $\theta$（法定存款準備率 Reserve ratio）作為準備金（Reserves, $R = \theta D$）時（Slides 22–27, 35–45）：

- **強力貨幣 / 準備貨幣 / 貨幣基數（High-powered Money / Monetary Base, $H$）**：
  $$H = CU^d + R^d = c M^d + \theta(1 - c) M^d = \left[ c + \theta(1 - c) \right] \$Y \cdot L(i)$$
  （其中 $c$ 為民眾持有通貨占總貨幣之比例，$1-c$ 為持有支票存款之比例）。
- **貨幣供給與貨幣乘數（Money Multiplier）**：
  令央行強力貨幣供給等於需求（$H = H^d$），可得廣義貨幣供給 $M^s$ 與強力貨幣 $H$ 之倍數關係：
  $$M^s = \underbrace{\frac{1}{c + \theta(1 - c)}}_{\text{貨幣乘數 (Money Multiplier } > 1\text{)}} \times H$$
  - 若民眾完全不持有通貨（$c = 0$），則貨幣乘數簡化為 **$\frac{1}{\theta}$**（例如法定準備率 $\theta = 10\%$，央行透過公開市場買債釋出 $\$100$ 強力貨幣，經銀行體系無窮等比存放款創造 $\$100 \times (1 + 0.9 + 0.9^2 + \dots) = \$1,000$，貨幣乘數為 $10$ 倍）。

---

## 4. 零利率底限 (ZLB)、流動性陷阱與現代貨幣政策工具

### 4.1 零利率底限与流動性陷阱（Liquidity Trap，Slides 30–33 & [[source-blanchard-chap-5|Ch.5 Slide 39]]）
- **零利率底限（Zero Lower Bound, ZLB）**：由於持有現金的名目報酬率為 `0%`，若債券名目利率轉為負值，人們將全數改持現金，故名目利率無法顯著低於零。
- **流動性陷阱（Liquidity Trap）**：
  - 當名目利率降至 $i \to 0$ 時，人們預期未來利率只會升不會降（亦即預期未來債券價格只會跌，持有債券面臨資本損失風險），因此在滿足交易需求後，人們寧可無限量持有貨幣。
  - 此時**貨幣需求的利率彈性趨近無限大（$\left|\frac{\partial L}{\partial i}\right| \to \infty$），貨幣需求曲線與 `LM` 曲線變為水平線**。
  - **政策失靈**：在流動性陷阱中，央行即使繼續擴大傳統貨幣供給（$M^s$ 右移，如 2008–2015 年 Fed 準備金暴增），新增資金全數被銀行超額準備與民間存款吸收，**名目利率維持在 0 不動，傳統貨幣政策三大工具（公開市場操作、重貼現率、法定準備率）失去進一步壓低短期利率的能力**。

### 4.2 現代央行的利率法則與充裕準備金工具（Slides 21, 32）
1. **泰勒法則（Taylor Rule，Slide 21 手寫筆記）**：現代央行通常直接設定目標名目政策利率 $R$（如美國聯邦基金利率 `FFR`），而非釘住貨幣數量：
   $$R = r + \pi + \alpha_1(\pi - \pi^*) + \alpha_2\left(\frac{Y - Y_f}{Y_f}\right)$$
   （根據實質利率 $r$、當期通膨與目標通膨缺口 $\pi - \pi^*$、以及產出缺口 $\frac{Y - Y_f}{Y_f}$ 動態調整）。
2. **充裕準備金架構下的新政策工具（Ample Reserves Framework，Slide 32）**：
   - 2008 年 QE 後銀行體系準備金極度充裕，微調準備金供給已無法改變利率，Fed 改以行政利率走廊控制 `FFR`：
     - **準備金利率（Interest on Reserves, `IOR`）**：央行付給銀行存款準備金的利率。
     - **隔夜附賣回協定利率（Overnight Reverse Repurchase Agreement, `ON RRP` rate）**：為貨幣市場基金等非銀行機構提供利率底限。

---

## 5. 關聯頁面與來源索引 (References)
- **相關概念**：[[is-lm-model-and-policy-mix|IS-LM 模型與財政貨幣政策搭配]]、[[extended-is-lm-and-financial-crisis|延伸型 IS-LM 模型、實質利率、風險溢酬與金融危機]]
- **延伸對比**：[[fiscal-vs-monetary-policy-in-is-lm|短期總體政策對比：財政政策 vs. 貨幣政策與政策組合實證]]
- **引用來源**：[[source-blanchard-chap-4|Blanchard Macroeconomics Ch.4 - Financial Markets]]、[[source-blanchard-chap-5|Blanchard Macroeconomics Ch.5 - The IS-LM Model]]
