---
title: "勞動市場：工資與價格設定模型 (Labor Market: Wage-Setting & Price-Setting Model)"
category: concept
tags:
  - macroeconomics
  - labor-market
  - ws-ps-model
  - natural-rate-of-unemployment
  - efficiency-wages
  - medium-run
created: 2026-11-16
updated: 2026-11-16
source_count: 2
status: active
---

# 勞動市場：工資與價格設定模型 (WS-PS Model)

## 1. 核心定義與時間維度定位

在總體經濟學從**短期（Short Run，需求決定產出、物價僵固）**邁向**中期（Medium Run，物價與工資充分調整）**時，**勞動市場（The Labor Market）**是決定一國「自然失業率（Natural Rate of Unemployment, $u_n$）」與「潛在產出（Potential Output, $Y_n$）」的核心引擎。

Blanchard 第 7 章透過勞資雙方的**工資設定關係（Wage-Setting Relation, `WS`）**與廠商的**價格設定關係（Price-Setting Relation, `PS`）**，解釋為何實質工資與均衡失業率是由勞動市場制度與產業競爭結構所共同決定。

---

## 2. 美國勞動市場的巨量流動（Labor Flows）與失業率風險

勞動市場表面上失業率看似平穩，底層卻無時無刻在發生驚人的雙向流動（依 1996–2014 年美國 CPS 每月平均數據，`[[source-blanchard-chap-7]]`）：
- **就業人口（Employed, $E$）**：$1.394$ 億人；**失業人口（Unemployed, $U$）**：$880$ 萬人（失業率 $u = 6.0\%$）；**非勞動力（Out of the Labor Force, $O$）**：$7,950$ 萬人。
- **每月離職總流量高達 $880$ 萬人**（佔總就業約 $6.3\%$）：其中约 $3/4$ 是直接跳槽（Job-to-job）或退休/就學，僅約 $1/4$（$200$ 萬人）進入失業池。
- **景氣衰退時企業如何縮減人力？**
  1. **首先大幅凍結招募（Hiring Freeze）**：降低失業者找到工作的機率，導致**平均失業期間（Duration of Unemployment）**拉長（正常期約 2–3 個月，2010 年金融海嘯後飆至 $35$ 週以上）。
  2. **其次才擴大裁員（Layoffs）**：提高在職勞工流失工作的風險。

---

## 3. 工資決定機制與效率工資理論（Efficiency Wages）

### 3.1 工資設定方程式（Wage Equation）
$$W = P^e F(u, z) \quad (-, +)$$

1. **為什麼工資取決於「預期物價水準 $P^e$」而非名目金額？**
   勞工在意的是薪水能買多少東西（實質購買力 $W/P$），廠商在意的是相對於產品售價的實質勞動成本（$W/P$）。由於名目工資通常在年初簽約、有效期達 1–3 年，雙方必須根據**預期物價 $P^e$** 來談判名目工資 $W$。
2. **為什麼失業率 $u$ 越高，工資越低？（$-$）**
   失業率高時，勞工一旦離職很難找到下一份工作（外部選擇價值下降），且企業不愁找不到替代人選，勞工議價能力（Bargaining Power）大幅減弱。
3. **制度綜合變數 $z$（$+$）**：
   包含**失業救濟金（Unemployment Insurance）**、**最低工資法（Minimum Wage）**、**就業保護法規（Employment Protection）**與工會力量。$z$ 越高，勞工失業的退路越好或開除成本越高，要求工資越高。

### 3.2 效率工資理論（Efficiency Wages）與亨利·福特日薪 5 美元案例
為什麼即使沒有工會，許多企業仍主動支付高於勞工保留工資（Reservation Wage）的薪水？
- **效率工資邏輯**：高薪能提高員工生產力、降低摸魚怠工（Shirking）誘因，並大幅減少員工離職帶來的招募與訓練成本（Turnover Costs）。
- **歷史經典案例：1914 年亨利·福特（Henry Ford）「日薪 5 美元」改革（`[[source-blanchard-chap-7]]` Slides 16–17）**：
  - 改革前（1913 年）：福特T型車裝配線工作枯燥繁重，當時業界日薪約 $\$2.30$，福特工廠**年離職率高達 $370\%$**（為維持 1.4 萬名人力，一年竟需招募 5.2 萬人！）。
  - 改革後（1914 年）：福特直接將日薪翻倍至 **$\$5.00$**（工時由 9 小時縮為 8 小時），結果**年離職率暴跌至 $16\%$**（1915 年），曠職率減半，單車生產成本反而大幅下降、利潤暴增！

---

## 4. 勞動市場均衡：WS-PS 模型與自然失業率（$u_n$）

在中期均衡下，人們對物價的預期完全實現（**$P^e = P$**）：

| 關係曲線 | 方程式 | 經濟意涵与決定因素 |
| :--- | :--- | :--- |
| **工資設定關係（`WS` 曲線）** | $$\frac{W}{P} = F(u, z)$$ | 向下傾斜：失業率 $u$ 越高，勞工敢要求的實質工資越低。制度變數 $z \uparrow$ 會使 `WS` 曲線上移。 |
| **價格設定關係（`PS` 曲線）** | $$P = (1 + m)W \implies \frac{W}{P} = \frac{1}{1 + m}$$ | 水平線：廠商依據獨佔力加成比例 $m$（Markup）定價，直接決定了廠商願意支付給勞工的**固定實質工資上限 $\frac{1}{1+m}$**。 |
| **中期勞動市場均衡（自然失業率 $u_n$）** | $$F(u_n, z) = \frac{1}{1 + m}$$ | 唯有當失業率調整到 **$u_n$** 時，勞工願意接受的實質工資才剛好等於廠商定價後願意給出的實質工資！ |

### 政策與結構變動的影響（Comparative Statics）
1. **失業救濟金提高（$z \uparrow$）**：在相同失業率下勞工要求更高工資 $\implies$ `WS` 曲線上移 $\implies$ 實質工資受限於 `PS` 不變（仍為 $\frac{1}{1+m}$），但**自然失業率上升（$u_n \uparrow$）**。
2. **反托拉斯執法放寬或油價暴漲（加成 $m \uparrow$）**：廠商提高售價加成 $\implies$ 實質工資被壓低（`PS` 水平線下移）$\implies$ 必須透過更高的失業率迫使勞工接受較低的實質工資，導致**實質工資下降、自然失業率上升（$u_n \uparrow$）**。

---

## 5. 關聯頁面與來源

- **原始教材來源**：
  - `[[source-blanchard-chap-7|Blanchard Ch.7：勞動市場 (The Labor Market)]]`
  - `[[source-blanchard-chap-8|Blanchard Ch.8：菲利浦曲線、自然失業率與通貨膨脹]]`
- **概念與延伸連結**：
  - `[[unemployment-and-labor-market|失業率、勞動參與率與勞動力市場]]`
  - `[[expectations-augmented-phillips-curve|附加預期的菲利浦曲線、自然失業率與通膨動態]]`
  - `[[is-lm-pc-medium-run-and-supply-shocks|IS-LM-PC 中期模型、貨幣中立性與供給衝擊]]`
  - `[[short-run-vs-medium-run-macro|總體經濟的短期與中期對決：需求驅動 vs. 供給約束]]`
