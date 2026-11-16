---
title: "通貨膨脹與物價指數 (Inflation & Price Indexes)"
category: concept
tags:
  - macroeconomics
  - inflation
  - price-index
  - cpi
  - pce
  - gdp-deflator
created: 2026-11-16
updated: 2026-11-16
source_count: 1
status: active
---

# 通貨膨脹與物價指數 (Inflation & Price Indexes)

## 1. 核心定義區辨 (Core Definitions)

根據 [[source-blanchard-chap-2|Blanchard Macroeconomics Ch.2]]：

- **通貨膨脹（Inflation）**：一般物價水準（General level of prices, $P_t$）的**持續性上漲（Sustained rise）**。
- **通貨膨脹率（Inflation Rate, $\pi_t$）**：物價水準上漲的比率：
  $$\pi_t = \frac{P_t - P_{t-1}}{P_{t-1}}$$
- **通貨緊縮（Deflation）**：一般物價水準持續性下跌（即負的通膨率，$\pi_t < 0$）。
- **反通膨 / 通膨減緩（Disinflation）**：通膨率仍在正值區間（$\pi_t > 0$，物價持續上漲），但**上漲速率放緩**（例如年增率由 `6%` 降至 `3%`）。
- **純粹通膨（Pure Inflation）**：理論假設所有商品價格與工資皆以**完全相同的比例**上漲，此時所有商品的**相對價格（Relative prices）完全不變**，實質購買力與資源配置不受影響。然而現實世界中**不存在純粹通膨**。

---

## 2. 拉氏指數 (Laspeyres) vs. 畢氏指數 (Paasche) 與替代偏誤

衡量跨期物價變動時，依數量權重（Basket weights）取自「基期」或「當期」，分為兩大基礎公式（Slides 49–51）：

| 指數類型 | 公式定義（$0$ 為基期，$1$ 為當期） | 對應指標代表 | 對通膨率的偏誤與原因 |
| :--- | :--- | :--- | :--- |
| **拉氏物價指數 (Laspeyres Price Index)** | $$L = \frac{\sum P_1 Q_0}{\sum P_0 Q_0} \times 100$$<br>（以**基期固定籃子數量 $Q_0$** 為權重） | **CPI（消費者物價指數）** | **高估通膨率（Overestimate）**：當某商品相對漲價時，消費者在現實中會改買較便宜的替代品（$Q_1 < Q_0$），但拉氏指數仍以高基期數量 $Q_0$ 計算，忽略替代效果而高估生活成本增幅。 |
| **畢氏物價指數 (Paasche Price Index)** | $$P = \frac{\sum P_1 Q_1}{\sum P_0 Q_1} \times 100$$<br>（以**當期實際籃子數量 $Q_1$** 為權重） | **GDP Deflator（GDP 平減指數）** | **低估通膨率（Underestimate）**：直接以消費者已經完成替代後的當期數量 $Q_1$ 計算，忽略消費者因被迫替代而損失的效用。 |

### 數值計算範例（Slide 51）
假設 2018 年為基期（Base Year），經濟體有 A、B 兩商品：
- **2018 年（基期 $0$）**：商品 A（$P_0=1, Q_0=4$）、商品 B（$P_0=3, Q_0=2$）
- **2019 年（當期 $1$）**：商品 A（$P_1=2, Q_1=3$）、商品 B（$P_1=4, Q_1=3$）

1. **Laspeyres Index ($L_{2019}$)**（固定使用 2018 年數量 $Q_0 = \{4, 2\}$）：
   $$L_{2019} = \frac{(\$2 \times 4) + (\$4 \times 2)}{(\$1 \times 4) + (\$3 \times 2)} \times 100 = \frac{8 + 8}{4 + 6} \times 100 = \frac{16}{10} \times 100 = 160 \quad (\text{通膨率 } +60\%)$$
2. **Paasche Index ($P_{2019}$)**（使用 2019 年數量 $Q_1 = \{3, 3\}$）：
   $$P_{2019} = \frac{(\$2 \times 3) + (\$4 \times 3)}{(\$1 \times 3) + (\$3 \times 3)} \times 100 = \frac{6 + 12}{3 + 9} \times 100 = \frac{18}{12} \times 100 = 150 \quad (\text{通膨率 } +50\%)$$
   $\rightarrow$ 清楚印證 **Laspeyres ($+60\%$) $>$ Paasche ($+50\%$)**。

---

## 3. GDP 平減指數 (GDP Deflator) 與成長率拆解恆等式

- **定義（Slides 46–47）**：
  $$P_t = \frac{\text{Nominal GDP}_t}{\text{Real GDP}_t} = \frac{\$Y_t}{Y_t} = \frac{\sum P_t Q_t}{\sum P_B Q_t}$$
- **名目 GDP、實質 GDP 與通膨率的動態近似關係**：
  由 $\$Y_t = P_t \times Y_t$，取變動率可得：
  $$\Delta\% \text{ Nominal GDP} \approx \Delta\% \text{ Price } (\pi_t) + \Delta\% \text{ Real GDP } (g_t)$$
- **關於 `CPI`、`PCE` 與 `GDP Deflator` 三者的深度橫向比較與聯準會政策選擇**，請參閱專題對比頁：[[cpi-vs-pce-vs-gdp-deflator|三大通膨與物價指標對比：CPI vs. PCE vs. GDP Deflator]]。

---

## 4. 為什麼經濟學家與央行重視通膨？ (Costs of Inflation & Optimal Target)

1. **所得與財富重分配效應（Income & Wealth Distribution）**：由於不同群體的薪資、退休金、資產與負債並非同步隨通膨調整（非純粹通膨），未預期通膨會造成債權人與債務人、固定薪資者與資產持有者之間的財富重分配。
2. **相對價格訊號扭曲與不確定性（Distortion & Uncertainty）**：高通膨伴隨高波動，加上累進稅制（Bracket creep）與價格調整頻率不一，會扭曲價格訊號，降低企業長期資本支出（`CAPEX`）與投資意願。
3. **最適通膨區間（Optimal Inflation Rate）**：多數總體經濟學家與現代央行認為，維持在 **`1% ~ 4%`**（如 Fed 與多數先進央行設定的 `2%` 目標）的溫和正通膨最佳，既能避免通縮螺旋，又能為實質利率調整保留緩衝空間。

---

## 5. 關聯頁面與來源索引 (References)
- **延伸對比**：[[cpi-vs-pce-vs-gdp-deflator|三大通膨與物價指標對比：CPI vs. PCE vs. GDP Deflator]]、[[fixed-base-vs-chain-linked-gdp|實質 GDP 衡量對比：定基法 vs. 連鎖法]]
- **相關概念**：[[gdp-and-national-income-accounting|GDP 與國民所得會計帳]]、[[okuns-law-and-phillips-curve|歐肯法則 (Okun's Law) 與菲利浦曲線 (Phillips Curve)]]
- **引用來源**：[[source-blanchard-chap-2|Blanchard Macroeconomics Ch.2 - A Tour of the Book]]
