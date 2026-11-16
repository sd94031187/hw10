---
title: "來源摘要：Blanchard Macroeconomics Ch.3 - The Goods Market"
category: source
source_path: "../../raw/Chap-3.pdf"
source_date: 2021-01-01
author: "Olivier Blanchard (Pearson, 8th Ed.) 及課程補充講義/手寫筆記"
tags:
  - source
  - macroeconomics
  - goods-market
  - consumption
  - multiplier
  - paradox-of-saving
created: 2026-11-16
updated: 2026-11-16
source_count: 1
status: active
---

# 來源摘要：Blanchard Macroeconomics Ch.3 — The Goods Market

- **原始檔案**：[Chap-3.pdf](../../raw/Chap-3.pdf)（共 46 頁投影片，含台灣 GDP 組成比重、比例稅乘數、加速效果與 IS 曲線練習補充）
- **教材版本**：Olivier Blanchard, *Macroeconomics*, Eighth Edition, Global Edition (Pearson, 2021)
- **消化日期 (Ingested)**：2026-11-16

---

## 1. 核心結論 (Key Takeaways)

1. **短期需求主導循環（Short-Run Demand Loop）**：在短期（年對年波動）中，**需求（Demand, $Z$）決定生產（Production, $Y$），生產創造等額所得（Income, $Y$），所得再回頭決定需求（特別是消費 $C$）**。
2. **GDP 支出面組成與台美結構差異**：
   - 總需求 $Z \equiv C + I + G + X - IM$（存貨投資 `Inventory investment` = 生產 $-$ 銷售，計入統計但非行為需求的一部分）。
   - **美國（2018）**：內需消費 $C$ 占 GDP 高達 **`68.0%`**，投資 $I$ 占 `17.5%`，政府支出 $G$ 占 `17.2%`，淨出口為 `-3.0%`（貿易赤字）。
   - **台灣（補充講義，Slides 6 & 8）**：出口 $X$ 占 GDP 比重高達 **`60% ~ 70%`**（淨出口長期為正），民間消費約占 `45% ~ 55%`；且台灣會計分類上，**民眾購買新屋屬於投資 $I$（固定資本形成）**，**政府基礎建設或購買機器設備亦歸入投資 $I$**（而非政府消費支出 $G$）。
3. **凱因斯消費函數與乘數效果（Multiplier Effect）**：
   - 消費行為方程式：$C = c_0 + c_1 Y_D = c_0 + c_1(Y - T)$，其中 $c_0$ 為自發性消費（Autonomous consumption，受未來預期與信心影響），$c_1$ 為邊際消費傾向（`MPC`, $0 < c_1 < 1$）。平均消費傾向 $APC = \frac{C}{Y_D} = \frac{c_0}{Y_D} + c_1 \ge MPC$。
   - 在封閉經濟且定額稅（Lump-sum tax）與固定投資（$I = \bar{I}$）下，均衡產出為：
     $$Y^* = \frac{1}{1 - c_1} \left[ c_0 + \bar{I} + G - c_1 T \right]$$
   - **不同稅制與財政條件下的乘數比較（課堂補充與手寫筆記，Slides 20–23）**：
     - 自發性支出乘數：$\frac{1}{1 - c_1} > 1$（幾何級數傳遞 $1 + c_1 + c_1^2 + \dots = \frac{1}{1-c_1}$）。
     - **平衡預算乘數（Balanced Budget Multiplier，當 $\Delta G = \Delta T$）**：$\frac{\Delta Y^*}{\Delta G}\big|_{\Delta G = \Delta T} = \frac{1 - c_1}{1 - c_1} = 1$（恆等於 1）。
     - **比例稅乘數（Proportional Tax，$T = T_0 + tY$）**：乘數縮小為 $\frac{1}{1 - c_1(1 - t)} < \frac{1}{1 - c_1}$（具備自動穩定器效果）。
4. **投資等於儲蓄（$I = S$）與節儉矛盾（Paradox of Saving）**：
   - 商品市場均衡條件 $Y = Z$ 完全等價於 **總投資 $=$ 總儲蓄（私人儲蓄 $S = Y - T - C$ $+$ 公共儲蓄 $T - G$）**：
     $$I = S + (T - G)$$
   - **節儉矛盾（Slides 38–40）**：當民眾因擔憂未來而試圖多儲蓄（減少自發性消費 $c_0 \downarrow$）時，會透過乘數效果導致均衡產出 $Y^* \downarrow$；
     - 若投資固定（$I = \bar{I}$），最終總儲蓄 $S$ **完全不變**（$c_0$ 下降剛好被誘發性儲蓄 $(1-c_1)Y$ 的減少完全抵銷）。
     - 若投資具**加速效果（Accelerator Effect，$I = I(Y)$ 且 $I'(Y) > 0$，Slide 40 補充）**，產出 $Y$ 下降會進一步壓低投資 $I(Y)$，導致**新的均衡總儲蓄反而比原本更低（$S_1 < S_0$）**！

---

## 2. 關鍵數據、案例與推導摘錄 (Key Data & Case Studies)

- **2008 年雷曼兄弟破產與消費函數左移（Slides 42–44）**：
  - 2008 Q3 雷曼兄弟破產引發「大蕭條（Great Depression）」Google 搜尋量暴增，消費者極度恐慌，即使當期可支配所得（$Y_D$）尚未明顯下滑，民眾仍大幅削減消費（特別是汽車等耐久財消費暴跌逾 `10%`），即**自發性消費 $c_0$ 大幅下降**。
- **IS 曲線代數推導練習（Slides 45–46）**：
  - 給定 $C = 100 + 0.75 Y_D$、$I = 50 - 25i$、$G = T = 50$：
  - $Y = 100 + 0.75(Y - 50) + 50 - 25i + 50 \implies 0.25Y = 162.5 - 25i \implies$ **IS 方程式：$Y = 650 - 100i$**。

---

## 3. 觸及與更新的 Wiki 頁面 (Linked Entities & Concepts)
- **新建/更新概念頁**：[[goods-market-and-multiplier|商品市場均衡、凱因斯消費函數與乘數效果]]、[[gdp-and-national-income-accounting|GDP 與國民所得會計帳]]
- **新建/更新對比頁**：[[fiscal-vs-monetary-policy-in-is-lm|短期總體政策對比：財政政策 vs. 貨幣政策與政策組合實證]]
