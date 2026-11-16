---
title: "來源摘要：Blanchard Macroeconomics Ch.4 - Financial Markets"
category: source
source_path: "../../raw/Chap-4.pdf"
source_date: 2021-01-01
author: "Olivier Blanchard (Pearson, 8th Ed.) 及課程補充講義/手寫筆記"
tags:
  - source
  - macroeconomics
  - financial-markets
  - money-demand
  - central-bank
  - liquidity-trap
  - money-multiplier
created: 2026-11-16
updated: 2026-11-16
source_count: 1
status: active
---

# 來源摘要：Blanchard Macroeconomics Ch.4 — Financial Markets

- **原始檔案**：[Chap-4.pdf](../../raw/Chap-4.pdf)（共 46 頁投影片，含台灣央行 M1A/M1B/M2 定義、泰勒法則、準備金架構新工具與貨幣乘數推導）
- **教材版本**：Olivier Blanchard, *Macroeconomics*, Eighth Edition, Global Edition (Pearson, 2021)
- **消化日期 (Ingested)**：2026-11-16

---

## 1. 核心結論 (Key Takeaways)

1. **貨幣需求（Money Demand）與語意陷阱區辨**：
   - **存量（Stock）vs. 流量（Flow）**：貨幣（Money）、累積儲蓄/財富（Savings / Financial wealth）為**存量變數**；所得（Income）、當期儲蓄（Saving）、實質投資（Investment，購買新資本財）為**流量變數**。
   - **名目貨幣需求方程式**：$M^d = \$Y \cdot L(i)$，與名目所得 $\$Y$（交易需求）成正比，與債券名目利率 $i$（持有貨幣的機會成本）成反比（$L'(i) < 0$）。
2. **公開市場操作（OMO）與債券價格—利率反向關係**：
   - 一年期貼現債券（Discount bond，面額 $\$100$，現價 $\$P_B$）之利率公式：
     $$i = \frac{\$100 - \$P_B}{\$P_B} \iff \$P_B = \frac{\$100}{1 + i}$$
   - **債券價格 $\$P_B$ 與利率 $i$ 呈嚴格反向關係**。
   - **擴張性公開市場操作（Expansionary OMO）**：央行在公開市場**買入債券** $\rightarrow$ 釋出強力貨幣 $H$、推升債券價格 $\$P_B \uparrow$ $\rightarrow$ 市場利率 $i \downarrow$。
   - **緊縮性公開市場操作（Contractionary OMO）**：央行**賣出債券** $\rightarrow$ 收回貨幣、壓低債券價格 $\$P_B \downarrow$ $\rightarrow$ 市場利率 $i \uparrow$。
3. **銀行準備金、強力貨幣（Monetary Base）與貨幣乘數（Money Multiplier）**：
   - 央行發行的負債稱為**央行貨幣 / 強力貨幣 / 準備貨幣（High-powered money / Monetary base, $H = CU + R$）**。
   - 當民眾持有通貨比例為 $c$（$CU^d = cM^d$）、支票存款比例為 $1-c$（$D^d = (1-c)M^d$），且商業銀行法定準備率為 $\theta$（$R^d = \theta D^d = \theta(1-c)M^d$）時，央行貨幣均衡條件為：
     $$H = [c + \theta(1 - c)] M^d \implies M^s = \frac{1}{c + \theta(1 - c)} H$$
   - 其中 $\frac{1}{c + \theta(1 - c)} > 1$ 即為**貨幣乘數（Money Multiplier）**（若民眾不持有現金 $c=0$，則簡化為 $\frac{1}{\theta}$）。
4. **零利率底限（Zero Lower Bound, ZLB）與流動性陷阱（Liquidity Trap）**：
   - 因持有現金利率為 $0$，名目利率無法顯著低於零（`ZLB`）。
   - 當名目利率降至 $i = 0$ 時，民眾在滿足交易需求後對持有貨幣與債券無差異，**貨幣需求曲線變為水平（貨幣需求的利率彈性趨近無限大）**。此時央行再透過傳統三大工具增加貨幣供給（如 2008–2015 年美國準備金暴增），均被家庭與銀行吸收，無法進一步壓低名目利率。
5. **台灣與美國貨幣總計數定義（Slide 46）及新舊貨幣政策工具（Slide 21, 32）**：
   - **台灣央行定義**：
     - `M1A` $=$ 通貨淨額 $+$ 支票存款 $+$ 活期存款（流動性最高）
     - `M1B` $=$ `M1A` $+$ 活期儲蓄存款（個人或非營利法人，常作為股市資金動能指標）
     - `M2` $=$ `M1B` $+$ 準貨幣（Quasi-money：定期存款、定期儲蓄存款、外匯存款、郵政儲金、附買回交易餘額、外國人新台幣存款、貨幣市場共同基金 `MMMF`）
   - **現代央行政策轉向**：現代央行（如 Fed）不再固定貨幣供給量，而是直接設定目標政策利率（可參考**泰勒法則 Taylor Rule**：$R = r + \pi + \alpha_1(\pi - \pi^*) + \alpha_2 \frac{Y - Y_f}{Y_f}$），並在**充裕準備金架構（Ample Reserves Framework）**下改用 **準備金利率（IOR）** 與 **隔夜附賣回利率（ON RRP）** 控制聯邦基金利率（`FFR`）。

---

## 2. 觸及與更新的 Wiki 頁面 (Linked Entities & Concepts)
- **新建/更新概念頁**：[[money-market-and-monetary-policy|貨幣市場、利率決定與央行政策工具]]
- **新建/更新對比頁**：[[fiscal-vs-monetary-policy-in-is-lm|短期總體政策對比：財政政策 vs. 貨幣政策與政策組合實證]]
