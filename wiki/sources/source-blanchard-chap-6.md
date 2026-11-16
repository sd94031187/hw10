---
title: "來源摘要：Blanchard Macroeconomics Ch.6 - Financial Markets II: The Extended IS-LM Model"
category: source
source_path: "../../raw/Chap-6.pdf"
source_date: 2021-01-01
author: "Olivier Blanchard (Pearson, 8th Ed.) 及課程補充講義/手寫筆記"
tags:
  - source
  - macroeconomics
  - extended-is-lm
  - fisher-equation
  - risk-premium
  - financial-crisis
  - securitization
created: 2026-11-16
updated: 2026-11-16
source_count: 1
status: active
---

# 來源摘要：Blanchard Macroeconomics Ch.6 — Financial Markets II: The Extended IS-LM Model

- **原始檔案**：[Chap-6.pdf](../../raw/Chap-6.pdf)（共 39 頁投影片，含費雪方程式推導、中性利率 $r^*$ 補充、2008 次貸危機與證券化 MBS/CDO/SIV/TARP 深度解析）
- **教材版本**：Olivier Blanchard, *Macroeconomics*, Eighth Edition, Global Edition (Pearson, 2021)
- **消化日期 (Ingested)**：2026-11-16

---

## 1. 核心結論 (Key Takeaways)

1. **名目利率 vs. 實質利率與費雪方程式（Fisher Equation，Slides 4–11）**：
   - 名目利率（$i_t$）以貨幣（美元）計價；**實質利率（$r_t$）以一籃子商品（購買力）計價**。
   - 精確關係式：$1 + r_t = \frac{1 + i_t}{1 + \pi_{t+1}^e}$；當利率與預期通膨不高時（忽略交叉項 $r_t \cdot \pi_{t+1}^e$），可得**費雪方程式（Fisher Equation）**：
     $$r_t \approx i_t - \pi_{t+1}^e \iff i_t \approx r_t + \pi_{t+1}^e$$
   - **事前（Ex-ante）vs. 事後（Ex-post）實質利率**：影響企業當期投資決策（進入 `IS` 曲線）的是扣掉「預期通膨 $\pi_{t+1}^e$」的**事前實質利率（Ex-ante real rate）**；而事後實際發生的購買力報酬則為 $i_t - \pi_{t+1}$（Ex-post real rate）。
   - **名目零利率底限（ZLB，$i_t \ge 0$）對實質利率的限制**：當 $i_t = 0$ 時，最低可能的實質利率為 **$r_t = -\pi_{t+1}^e$**（若發生通縮 $\pi^e < 0$，實質利率將被迫為正值，加深衰退！）。
2. **風險與風險溢酬（Risk and Risk Premia，Slides 12–14）**：
   - 風險中立下，無風險公債報酬 $(1+i)$ 應等於具違約機率 $p$ 之風險債券預期報酬 $(1-p)(1+i+x) + p(0)$，解得**風險溢酬（Risk Premium, $x$）**：
     $$x = \frac{(1 + i)p}{1 - p} > 0$$
   - 實務上，風險溢酬 $x$ 取決於兩大因素：(1) **違約機率（信用風險 $p$）**；(2) **投資人的風險趨避程度（Degree of risk aversion）**。2008 年 9 月次貸危機爆發時，`BBB` 級企業債殖利率相對於 10 年期美國公債與 `AAA` 債券暴增（信用利差飆升）。
3. **金融中介、高槓桿、賤售（Fire Sales）與銀行擠兌（Bank Runs，Slides 15–18）**：
   - **資本比率（Capital ratio）**$= \frac{\text{Capital}}{\text{Assets}}$；**槓桿比率（Leverage ratio）**$= \frac{\text{Assets}}{\text{Capital}} = \frac{1}{\text{Capital ratio}}$（例如資產 100、負債 80、自有資本 20，則槓桿倍數為 `5 倍`）。
   - 槓桿愈高，預期股東權益報酬率愈高，但資產價值微幅下跌即可能導致**資不抵債（Insolvency，淨值 $\le 0$）**與道德風險（Moral hazard）。
   - 若銀行資產流動性極低（如長期放款），而負債流動性極高（如隨時可提領之活期存款），一旦存款人懷疑銀行資產減損而集中提領，銀行被迫以遠低於真實價值的**賤售價格（Fire sale prices）**拋售資產，使流動性危機瞬間演變為破產與**銀行擠兌（Bank runs）**。防範機制包含：聯邦存款保險（FDIC，1934 年設立，2008 年由 \$10 萬調升至 \$25 萬）與央行最後貸款者（Lender of last resort）貼現窗口。
4. **延伸型 IS-LM 模型（Extended IS-LM）與中性利率（Neutral Rate $r^*$，Slides 19–25）**：
   - 明確區分央行控制的**實質政策利率（Policy rate, $r = i - \pi^e$）**與民間企業/家庭實際面臨的**實質借款利率（Borrowing rate $= r + x$）**：
     $$\text{IS Relation}: \quad Y = C(Y - T) + I(Y, \ r + x) + G$$
     $$\text{LM Relation}: \quad r = \bar{r}$$
   - **中性利率（Neutral Rate of Interest, $r^*$，Slides 21–23 補充）**：使短期產出等於潛在產出（$Y = Y_f$）且通膨穩定維持在目標（`2%`）時的實質利率。
     - 當實際實質利率 $r < r^*$（或名目政策利率 $<$ $r^* + \pi^e$）：代表**寬鬆（Accommodative）**貨幣政策立場。
     - 當實際實質利率 $r > r^*$（或名目政策利率 $>$ $r^* + \pi^e$）：代表**緊縮/限制性（Restrictive）**貨幣政策立場。
   - **金融衝擊（Financial Shock，$x \uparrow$）**：當金融危機導致違約風險與風險溢酬 $x$ 暴增時，`IS` 曲線大幅左移，產出重挫。此時央行必須大幅調降政策利率 $r$（甚至降至負實質利率），並透過**非傳統貨幣政策（量化寬鬆 `QE`）**直接買入中長期債券與 MBS 以壓低風險溢酬 $x$（使 `IS` 右移回穩）。
5. **2008 年次貸金融危機的完整傳導鏈（Slides 26–39）**：
   - **起因**：2000–2006 低利率助長房價泡沫與**次級房貸（Subprime mortgages）**，銀行透過**資產證券化（Securitization：MBS 與分券 CDO — Senior AAA / Mezzanine BBB / Junior B）**及表外**結構型投資工具（SIVs，依賴短期批發融資 Wholesale funding 買入長期 ABS）**規避資本監管並將槓桿放到極限。
   - **崩潰**：2006 年後房價反轉下跌，房貸淪為**負資產（Underwater）**，次貸大規模違約引爆 CDO 崩盤與批發融資斷鏈。
   - **三大政策救市組合**：(1) **金融政策**：提高存款保險上限至 \$25 萬、Fed 擴大擔保品流動性融通、財政部推出 **不良資產救助計畫（TARP）** 剝離有毒資產並直接注資大型銀行補充資本（降低槓桿率）；(2) **貨幣政策**：2008 年 12 月將 FFR 降至零（ZLB）並啟動 `QE`；(3) **財政政策**：2009 年 2 月通過 **\$7,800 億美元《美國復甦與再投資法案（ARRA）》** 減稅與擴大支出。

---

## 2. 觸及與更新的 Wiki 頁面 (Linked Entities & Concepts)
- **新建/更新概念頁**：[[extended-is-lm-and-financial-crisis|延伸型 IS-LM 模型、實質利率、風險溢酬與金融危機]]、[[is-lm-model-and-policy-mix|IS-LM 模型與財政貨幣政策搭配]]
- **新建/更新對比頁**：[[fiscal-vs-monetary-policy-in-is-lm|短期總體政策對比：財政政策 vs. 貨幣政策與政策組合實證]]
