---
title: "Blanchard Ch.10：經濟成長的事實 (The Facts of Growth)"
category: source
source_path: "../../raw/Chap-10.pdf"
source_date: 2026-11-16
author: "Olivier Blanchard (Macroeconomics, 8th Edition)"
tags:
  - source
  - macroeconomics
  - economic-growth
  - ppp
  - easterlin-paradox
  - malthusian-trap
  - convergence
  - solow-model
created: 2026-11-16
updated: 2026-11-16
source_count: 1
status: active
---

# Blanchard Ch.10：經濟成長的事實 (The Facts of Growth)

- **原始檔案**：[Chap-10.pdf](../../raw/Chap-10.pdf)（共 50 頁，含課堂教授手寫推導與圖表解析）
- **核心主題**：進入總體經濟學的**長期（Long Run）**核心議題——**經濟成長（Economic Growth）**。介紹跨國生活水準衡量的**購買力平價（Purchasing Power Parity, PPP）**、探討「金錢能否買到快樂（Easterlin Paradox vs. Stevenson-Wolfers 實證）」、回顧人類兩千年經濟史（馬爾薩斯陷阱 Malthusian Trap 與工業革命）、檢驗富裕國家與亞洲四小龍的**收斂假說（Convergence）**，並建立**索洛成長模型（Solow Growth Model）**的總體生產函數與兩大成長來源（資本累積 vs. 技術進步）。

---

## 1. Gate 1 前置驗算與跨章節檢查紀錄

- **美國長期成長倍數驗算（Slide 5）**：
  - 1890 年至 2016 年，美國實質 GDP 成長 **51 倍**，人口由 $6,300$ 萬增至 $3.2$ 億（約 $5.08$ 倍），因此**實質人均 GDP（Real GDP per person）成長約 $\frac{51}{5.08} \approx 10$ 倍**，無誤。
- **美俄購買力平價（PPP）算例驗算（Slide 8）**：
  - **美國**：人均消費 $\$20,000$（買 1 台汽車 $\$10,000$ + 1 年食物 $\$10,000$）。
  - **俄羅斯**：人均消費 $120,000$ 盧布（買 0.07 台汽車 $42,000$ 盧布［每台車 $600,000$ 盧布］+ 1 年食物 $78,000$ 盧布）。
  - **匯率法（Market Exchange Rate, $\$1 = 60$ 盧布）**：俄羅斯人均消費 $= \frac{120,000}{60} = \$2,000$，僅為美國的 **$\frac{2,000}{20,000} = 10\%$**。
  - **購買力平價法（PPP，統一以美國價格計價）**：俄羅斯一籃子消費價值 $= 0.07 \times \$10,000 + 1 \times \$10,000 = \$700 + \$10,000 = \$10,700$，為美國的 **$\frac{10,700}{20,000} = 53.5\%$**。驗算完全正確！

---

## 2. 跨國生活水準衡量：購買力平價（PPP，Slides 6–9）

- **為什麼不能直接用市場匯率換算各國人均 GDP？**
  1. 匯率受國際資本流動與匯市投機影響，波動劇烈，但國內實質生活水準不會一夕暴跌。
  2. **巴拉薩—薩繆爾森效應（Balassa-Samuelson Effect / 非貿易財價格差異）**：人均 GDP 越低的開發中國家，勞力密集的服務業與食物等非貿易財（Non-tradables）價格越便宜。若直接用市場匯率換算，會嚴重**低估**開發中國家的實質購買力（如上例俄羅斯從 $53.5\%$ 被低估為 $10\%$）。
- **PPP（國際元 International Dollars）**：採用一套共同的基準價格（通常為美國價格）重新加權計算各國實質產出與消費。

---

## 3. 經濟成長能帶來快樂嗎？（Does Money Lead to Happiness? Slides 10–19）

| 研究學派 / 學者 | 核心主張與發現 | 關鍵方法論差異 |
| :--- | :--- | :--- |
| **伊斯特林悖論（Easterlin Paradox, 1974）**<br>（Slides 10–15） | 1. 在同一個國家內部，富人比窮人快樂（相對所得重要）。<br>2. 但在富裕國家之間橫向比較，或隨時間縱向追蹤，人均 GDP 翻倍並未提高平均快樂程度（邊際快樂遞減至零）。 | 早期跨國樣本較少，且橫軸直接採用「人均 GDP 絕對金額（線性刻度）」。 |
| **Stevenson & Wolfers (2008) 全球實證**<br>（Slides 16–19，涵蓋 131 國 Gallup World Poll） | **駁斥伊斯特林悖論**！無論在窮國或富國、跨國比較或國內比較，**人均實質所得（對數刻度）與生活滿意度（Life Satisfaction）皆呈現高度且穩定的正相關**，沒有所謂「超過某個所得門檻錢就不再買得到快樂」的飽和點。 | 橫軸改用**「PPP 人均 GDP 的對數刻度（Log Scale）」**——代表所得每「翻倍（增加相同百分比）」，生活滿意度就會提升固定幅度。 |

---

## 4. 兩千年經濟史與跨國收斂（Convergence，Slides 20–35）

1. **三個歷史階段（Slides 20–24）**：
   - **馬爾薩斯陷阱時期（Malthusian Era，西元元年羅馬帝國至 1500 年）**：長達 1,500 年間，全球人均產出幾乎是**零成長**！因為農業土地報酬遞減，只要技術偶爾進步使糧食增加，死亡率就會下降、人口等比例膨脹，把人均糧食重新壓回生存邊緣（Subsistence level）。
   - **後馬爾薩斯時期（1500–1700 年）**：歐洲人均 GDP 年成長率微升至 $0.1\%$/年。
   - **現代經濟成長（工業革命後，1820 年至今）**：技術進步速度超越人口成長，美國 1950–2017 年人均實質 GDP 年均複合成長率達 $2.0\%$（67 年翻了 $3.8$ 倍）。
2. **富裕國家與新興經濟體的「收斂假說（Convergence）」檢驗（Slides 25–35）**：
   - **OECD 富裕俱樂部（無條件收斂，Slides 25–28）**：1950 年人均 GDP 越低的國家（如日本），1950–2017 年平均成長率越高（日本年成長 $4.1\%$，實質人均產出翻了 $15.9$ 倍，從美國的 $19\%$ 追趕至 $73\%$）。
   - **亞洲奇蹟（Asian Four Tigers & China，Slides 31–33）**：台灣、新加坡、香港、南韓（亞洲四小龍）在 1960 年人均 GDP 僅為美國的 $18\%$，至 2009 年已追趕至美國的 **$83\%$**；中國更以年均 $4.4\%$–$8\%+$ 的高速成長快速追趕。
   - **全球視角與非洲困境（條件收斂 Conditional Convergence，Slides 29–35）**：若將全球所有國家放在一起（Slide 29），並不存在無條件收斂——許多非洲國家（如辛巴威、剛果、中非共和國）1960 年很窮，但接下來半世紀人均產出反而倒退（負成長），主因在於戰爭、制度崩潰與缺乏產權保護。

---

## 5. 索洛成長模型導論：總體生產函數與兩大引擎（Slides 36–50）

1. **總體生產函數（Aggregate Production Function）**：
   $$Y = F(K, N)$$
   其中 $Y$ 為總產出，$K$ 為實體資本存量（機器、廠房、設備），$N$ 為勞動投入。函數形式 $F(\cdot)$ 由**技術水準（State of Technology）**決定。
2. **兩大核心性質（Slides 38–42）**：
   - **規模報酬固定（Constant Returns to Scale, CRTS）**：將資本與勞動同時擴大 $x$ 倍，產出也剛好擴大 $x$ 倍：
     $$xY = F(xK, xN)$$
     令 $x = \frac{1}{N}$，即可將總體生產函數轉化為**「每位勞工平均產出（Output per Worker）」對「每位勞工平均資本（Capital per Worker）」的集約形式（Intensive Form）**：
     $$\frac{Y}{N} = F\left(\frac{K}{N}, 1\right) \equiv f\left(\frac{K}{N}\right)$$
   - **資本邊際報酬遞減（Decreasing Returns to Capital）**：在勞動 $N$ 固定下，每多給勞工一台電腦或機器（$K/N \uparrow$），所能增加的產出越來越少（函數曲線越來越平緩，$f'(k) > 0, f''(k) < 0$）。
3. **長期成長的核心定理（Slides 43–50）**：
   - **單靠資本累積（提高儲蓄率 $s$）無法維持永久的經濟成長**：因為資本邊際報酬遞減，當資本存量越來越高，需要拿去彌補折舊的儲蓄比例越來越大，最終經濟必定停留在某個穩態水準。
   - **唯有持續的「技術進步（Technological Progress）」**（使生產函數 $F(K,N)$ 不斷向上移動），才能克服報酬遞減，維持人均產出的長期持續成長。

---

## 6. 關聯 Wiki 頁面

- `[[economic-growth-ppp-and-happiness|長期經濟成長事實：購買力平價 (PPP)、快樂經濟學與跨國收斂]]`
- `[[solow-growth-model-and-golden-rule|索洛成長模型 (Solow Model)、穩態與黃金法則儲蓄率]]`
- `[[gdp-and-national-income-accounting|GDP 與國民所得會計 (GDP & National Income Accounting)]]`
