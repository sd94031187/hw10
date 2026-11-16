---
title: "來源摘要：Blanchard Macroeconomics Ch.5 - Goods and Financial Markets: The IS-LM Model"
category: source
source_path: "../../raw/Chap-5.pdf"
source_date: 2021-01-01
author: "Olivier Blanchard (Pearson, 8th Ed.) 及課程補充講義/手寫筆記"
tags:
  - source
  - macroeconomics
  - is-lm
  - fiscal-policy
  - monetary-policy
  - crowding-out
created: 2026-11-16
updated: 2026-11-16
source_count: 1
status: active
---

# 來源摘要：Blanchard Macroeconomics Ch.5 — Goods and Financial Markets: The IS-LM Model

- **原始檔案**：[Chap-5.pdf](../../raw/Chap-5.pdf)（共 63 頁投影片，含 IS/LM 斜率全微分推導、投資利率彈性、排擠效果、2001 衰退與 1990s 柯林頓赤字縮減案例）
- **教材版本**：Olivier Blanchard, *Macroeconomics*, Eighth Edition, Global Edition (Pearson, 2021)
- **消化日期 (Ingested)**：2026-11-16

---

## 1. 核心結論 (Key Takeaways)

1. **內生投資函數與 IS 曲線（商品市場均衡）**：
   - 放棄第 3 章投資外生固定的假設，將投資設定為**產出（或銷售）$Y$ 的增函數**與**利率 $i$ 的減函數**：
     $$I = I(Y, i), \quad (+, -)$$
   - 商品市場均衡條件（`IS Relation`）：$Y = C(Y - T) + I(Y, i) + G$。
   - **IS 曲線負斜率與移動**：利率 $i \uparrow \implies$ 投資 $I \downarrow \implies$ 透過乘數使均衡產出 $Y \downarrow$，故 `IS` 曲線呈負斜率。凡在給定利率下增加總需求的因素（如 $G \uparrow$、$T \downarrow$、消費者信心 $c_0 \uparrow$）皆使 `IS` 右移；反之左移。
   - **IS 斜率的全微分與彈性決定因素（Slides 11–14 補充）**：
     $$\left.\frac{\partial i}{\partial Y}\right|_{IS} = \frac{1 - C_{Y_D} - I_Y}{I_i} \quad (\text{若簡化 } I=I(i) \text{ 則為 } \frac{1 - c_1}{I_i} = \frac{1 - c_1}{\varepsilon_i^I} \frac{i}{I} < 0)$$
     當**投資的利率彈性 $|\varepsilon_i^I|$ 愈大**或**邊際消費傾向 $c_1$（乘數）愈大**時，利率微幅下降即可帶動產出大幅增加，`IS` 曲線愈**平坦（Flatter）**，此時貨幣政策調息刺激產出的效果愈強。
2. **實質貨幣供需與 LM 曲線（金融市場均衡）**：
   - 將名目貨幣供需同除以物價水準 $P$，得實質貨幣供需均衡（`LM Relation`）：$\frac{M}{P} = Y \cdot L(i)$。
   - **兩種央行政策設定下的 LM 曲線**：
     - **現代央行（利率目標制，正文 Slides 16–24）**：央行直接選擇目標利率 $i = \bar{i}$（並自動調整貨幣供給達成之），故 `LM` 為一條在 $\bar{i}$ 的**水平線**。此時擴張性財政政策（$G \uparrow$）**不會產生利率上升的排擠效果（No crowding-out effect）**。
     - **傳統貨幣供給目標制（固定 $M$，附錄 Slides 36–45）**：$Y \uparrow \implies$ 實質貨幣需求右移 $\implies$ 均衡利率 $i \uparrow$，故 `LM` 呈**正斜率**：
       $$\left.\frac{di}{dY}\right|_{LM} = -\frac{L(i)}{Y \cdot L_i} > 0 \quad (L_i = \frac{\partial L}{\partial i} < 0)$$
       當貨幣需求對利率愈敏感（$|L_i|$ 愈大），`LM` 愈平坦；當 $i \to 0$ 陷入**流動性陷阱**（$|L_i| \to \infty$）時，`LM` 左端呈現水平段。
3. **財政政策對投資的排擠（Crowding-out）與擠入（Crowding-in）模糊性（Slides 43–47）**：
   - 在正斜率 `LM` 下，若政府擴大赤字（$G \uparrow$ 或 $T \downarrow$），產出 $Y \uparrow$（透過加速效果推升投資），但同時利率 $i \uparrow$（壓抑投資）；在不確知 $I(Y, i)$ 具體函數形式下，投資增減方向不確定（若投資下降稱為 `Crowding out`，若因 $Y$ 成長帶動投資上升稱為 `Crowding in`）。
   - 但若搭配央行貨幣政策（如**財政整頓縮減赤字 $G \downarrow / T \uparrow$ 搭配央行降息 $i \downarrow$** 維持產出 $Y$ 不變），則由 $I = S + (T - G)$ 可知：私人儲蓄 $S$ 不變、公共儲蓄 $(T-G) \uparrow$，**投資 $I$ 必定上升**（如 1990 年代美國柯林頓政府與 Fed 主席 Greenspan 的政策組合）。
4. **計量實證：IS-LM 模型的動態調整時間差（Slides 28–35）**：
   - 美國實證顯示，當 Fed 將聯邦基金利率（`FFR`）調升 `1%`：零售銷售與產出（GDP）在隨後數季明顯下滑（產出在約 **4～8 季**達到最大跌幅約 `-0.6%`），失業率上升；但**物價水準（Price level）在前 6 個季度（1.5 年）幾乎完全不變**，6 季後才開始緩慢下滑——這強力印證了 `IS-LM` 模型在短期（1.5 年內）假設「物價水準固定」的合理性！

---

## 2. 觀點分歧與跨章節數據修正紀錄 (Contradiction & Revision Tracking)

- **2001 年美國經濟衰退的季度 GDP 數據修正（對比 Ch.2 Slide 22 vs. Ch.5 Slide 48）**：
  - 在 [[source-blanchard-chap-2|Ch.2 Slide 22]] 中，早期初版數據指稱「2001 年前三個季度（Q1–Q3）GDP 成長率皆為負值，符合連續兩季負成長的衰退慣例」。
  - 但在本章 **Slide 48–49（Focus: The U.S. Recession of 2001）** 中明確指出：根據事後**修正後數據（Revised data, Figure A1）**，2001 年 Q2 的實質 GDP 季增年率其實是**微幅正成長**（僅 2000 Q3、2001 Q1 與 2001 Q3 為負值，並未出現連續兩季負成長）！儘管如此，美國國家經濟研究局（`NBER`）綜合評估非農就業與工業生產後，仍認定 2001 年 3 月至 12 月為正式衰退期。

---

## 3. 觸及與更新的 Wiki 頁面 (Linked Entities & Concepts)
- **新建/更新概念頁**：[[is-lm-model-and-policy-mix|IS-LM 模型與財政貨幣政策搭配]]、[[gdp-and-national-income-accounting|GDP 與國民所得會計帳]]
- **新建/更新對比頁**：[[fiscal-vs-monetary-policy-in-is-lm|短期總體政策對比：財政政策 vs. 貨幣政策與政策組合實證]]
