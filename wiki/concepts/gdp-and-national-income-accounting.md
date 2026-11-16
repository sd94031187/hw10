---
title: "GDP 與國民所得會計帳 (GDP & National Income Accounting)"
category: concept
tags:
  - macroeconomics
  - gdp
  - national-income
  - hedonic-pricing
created: 2026-11-16
updated: 2026-11-16
source_count: 3
status: active
---

# GDP 與國民所得會計帳 (GDP & National Income Accounting)

## 1. 定義與核心邏輯 (Definition & Core Logic)

- **GDP（Gross Domestic Product，國內生產毛額）**：一國經濟體在**特定期間內**所生產之**最終財貨與服務（Final goods and services）**的市場價值總和。
- **中間財（Intermediate Goods）的排除原則**：
  - 定義：用於生產其他商品而在當期消耗掉的財貨（例如汽車廠向鋼鐵廠採購的鋼材）。
  - 為何不計入 GDP：避免**重複計算（Double counting）**。若將鋼鐵廠與汽車廠合併為單一企業，其最終對外銷售額即為最終財價值。
- **進口品（Imports）的扣除原則**：無論是企業購買進口中間財或消費者購買進口最終財，進口品皆屬於外國生產之 GDP，計算本國 GDP 時必須扣除。

---

## 2. GDP 的三面等價計算方法 (Three Approaches to GDP)

國民所得會計帳中，**總生產（Aggregate Production）$\equiv$ 總所得（Aggregate Income）$\equiv$ 總支出（Aggregate Expenditure）**：

| 計算面向 | 核心定義與公式 | 雙廠商範例（鋼鐵廠營收 \$100：工資 \$80、利潤 \$20；汽車廠營收 \$200：鋼材 \$100、工資 \$70、利潤 \$30） |
| :--- | :--- | :--- |
| **1. 生產面法 (Production / Value-Added Approach)** | **方法 1（最終財加總）**：僅加總最終財與服務價值。<br>**方法 2（附加價值法 Value-Added）**：各生產階段「產出價值 $-$ 中間投入價值」之總和。 | **最終財**：僅計汽車銷售 = `\$200`<br>**附加價值**：鋼鐵廠 `\$100 - \$0 = \$100` $+$ 汽車廠 `\$200 - \$100 = \$100` $\rightarrow$ 合計 `\$200` |
| **2. 所得面法 (Income Approach)** | 經濟體內所有生產要素所得（勞動報酬 $+$ 資本/利潤所得 $+$ 地租 $+$ 利息）加上間接稅淨額與折舊。 | **勞動所得（Wages）**：`\$80 + \$70 = \$150`<br>**資本/利潤所得（Profit）**：`\$20 + \$30 = \$50`<br>$\rightarrow$ 合計 `\$200` |
| **3. 支出面法 (Expenditure Approach)** | 最終財貨與服務被購買/支出的總價值：<br>$$Y = C + I + G + X - M$$ | $C$（民間消費）$+$ $I$（國內投資）$+$ $G$（政府支出）$+$ $X$（出口）$-$ $M$（進口，因 $C, I, G$ 中包含進口品故須減除） |

---

## 3. 國民所得家族指標與台灣主計總處架構 (National Income Metrics)

根據 [[source-blanchard-chap-2|Blanchard Ch.2 補充講義]]（台灣行政院主計總處定義）：

### 3.1 從 GDP 到 GNI、NNI、NI 與 PI 的推導鏈
1. **GNI（Gross National Income，國民所得毛額，即 GNP 國民生產毛額）**：
   $$\text{GNI} = \text{GDP} + \text{國外要素所得收入淨額 (NFI)}$$
   - $\text{NFI} = \text{本國生產要素在國外之所得} - \text{外國生產要素在本國之所得}$。
2. **NDP（國內生產淨額）與 NNI（國民所得淨額 / 按市價計算之國民所得）**：
   $$\text{NDP} = \text{GDP} - \text{折舊 (Depreciation)}$$
   $$\text{NNI (按市價計算之國民所得)} = \text{GNI} - \text{折舊 (Depreciation)}$$
   - *扣除折舊之原因*：固定資本在生產過程中會有耗損（重置成本），扣除折舊後才代表經濟體真正淨增加的產出與所得。
3. **NI（National Income，按要素成本計算之國民所得）**：
   $$\text{NI} = \text{NNI} - \text{生產及進口稅淨額（間接稅淨額）}$$
   - 其中：$\text{間接稅淨額} = \text{間接稅} - \text{政府補貼}$。
   - **間接稅 vs. 按市價/按要素成本**：政府對生產、銷售或進口課徵之稅捐（間接稅），廠商視為生產成本並**轉嫁**給消費者，構成市場售價的一部分。因此包含間接稅淨額者稱為「按市價計算」，扣除後則還原為純粹歸屬於生產要素（受僱人員報酬 $+$ 營業盈餘［利息 $+$ 地租 $+$ 稅後利潤］）的「按要素成本計算之國民所得」。
   - **不計入國民所得之項目**：凡**非由生產而發生**之所得（如資產重估增值、國際間贈與、公債利息收入、移轉性支付）均不可計入 NI。
4. **PI（Personal Income，個人所得）與可支配所得**：
   $$\text{PI} = \text{NI} - \text{勞而不獲} + \text{不勞而獲}$$
   - **減項（勞而不獲，參與生產但未分給個人）**：營利事業所得稅、社會保險保費、公司未分配盈餘、企業罰款、政府財產所得。
   - **加項（不勞而獲，未參與當期生產但個人實際收到）**：失業保險、社會福利金、退休年金、政府補助金、公債利息、國內外移轉收入淨額。
   - **國民可支配所得** $=$ 按市價計算之國民所得（NNI）$+$ 國外經常移轉收入淨額。

---

## 4. 名目 GDP vs. 實質 GDP 與特徵定價法 (Nominal vs. Real GDP)

- **名目 GDP（Nominal GDP，教材記號為 $\$Y_t$）**：以**當期價格（Current prices）**計算之最終財總值：
  $$\$Y_t = \sum_{i=1}^{n} p_i^t q_i^t$$
- **實質 GDP（Real GDP，教材記號為 $Y_t$）**：以**固定基期價格（Base-year / Constant prices）**或**連鎖量指數（Chained dollars）**計算，用以衡量真正排除物價干擾後的「總產出數量變動」：
  $$Y_t = \sum_{i=1}^{n} p_i^c q_i^t$$
  - 在**基期年（Base year）**當年度，名目 GDP 恆等於實質 GDP（$\$Y_t = Y_t$）。
  - 關於基期選擇導致成長率變動的難題與解法，詳見專題對比：[[fixed-base-vs-chain-linked-gdp|實質 GDP 衡量對比：定基法 vs. 連鎖法]]。
- **特徵定價法（Hedonic Pricing，品質調整定價）**：
  - 針對電腦、半導體等技術快速進步的產品，美國商務部（BEA）採用 `Hedonic Pricing`，將商品視為一組特徵（運算速度、記憶體容量等）的集合。
  - **實證案例（1999 年以來筆記型電腦）**：筆電品質（運算服務效能）平均每年提升 `20%`，名目美元售價平均每年下降 `7%`，因此**經品質調整後的實質價格（Quality-adjusted price）平均每年下降 `27%`**（$20\% + 7\%$）。

---

## 5. 支出面 GDP 組成結構：美國 vs. 台灣會計分類與比重對比

根據 [[source-blanchard-chap-3|Blanchard Ch.3 (Slides 4–8)]]：

| 支出組成項目 | 定義與會計歸類重點（含台灣主計總處特殊規定） | 美國占 GDP 比重 (2018，總額 \$20.5 兆) | 台灣占 GDP 比重 (2014–2023 區間) |
| :--- | :--- | :---: | :---: |
| **民間消費 ($C$)** | 消費者購買之財貨（耐久財、非耐久財）與服務。<br>📌 *注意*：**民眾購買新屋不計入消費 $C$，而是計入住宅投資 $I$**。 | **`68.0%`** (\$13,951B) | **`~45% – 55%`** |
| **國內投資 ($I$)** | **固定投資（Fixed investment）**：非住宅投資（企業購買廠房、機器設備、電腦軟體）$+$ 住宅投資（民眾購買新屋）。<br>📌 *台灣補充*：**政府基礎建設支出或購買機器設備在台灣歸屬於投資 $I$**（固定資本形成），而非 $G$。 | **`17.5%`** (\$3,595B)<br>*(非住宅 13.6% + 住宅 3.8%)* | **`~20% – 28%`** |
| **政府支出 ($G$)** | 各級政府購買之財貨與服務（含公務員薪資等政府消費性支出）。<br>📌 *排除項目*：**不包含政府移轉性支付（Medicare、社福金）與公債利息支出**（此二項非購買當期商品服務，計入個人所得之「不勞而獲」）。 | **`17.2%`** (\$3,522B) | **`~13% – 15%`** |
| **淨出口 ($X - IM$)** | 出口（$X$，外國人購買本國產品）減去進口（$IM$，本國人購買外國產品）。$X > IM$ 為貿易順差（Trade surplus），$X < IM$ 為貿易逆差（Trade deficit）。 | **`-3.0%`** (-\$625B)<br>*(出口 12.4%, 進口 15.4%)* | **`+10% – 18%`**<br>*(出口占 60%~70%，進口占 50%~58%)* |
| **存貨投資 (Inventory Investment)** | $\text{當期生產} - \text{當期銷售}$（生產 100 台車僅賣出 90 台，則 10 台計入存貨投資 $+I$）。 | **`0.2%`** (\$56B) | 隨景氣循環小幅波動 |

---

## 6. 經濟成長率、衰退定義與跨章節數據修正追蹤 (GDP Growth & Contradictions)

- **實質 GDP 成長率**：$g_t = \frac{Y_t - Y_{t-1}}{Y_{t-1}}$。
- **經濟衰退（Recession）的慣例判準**：總體經濟學界與市場慣例常將 **「實質 GDP 連續至少兩個季度負成長（at least two consecutive quarters of negative growth）」** 視為衰退的經驗法則，但美國官方認定機構為 **NBER（國家經濟研究局）**。

> [!WARNING] 觀點分歧 / 數據衝突：2001 年美國 Y2K 衰退的季度 GDP 數據修正 (2026-11-16 更新)
> - **先前論點 / 初版數據（根據 [[source-blanchard-chap-2|Blanchard Ch.2 Slide 22]]）**：
>   - 宣稱 2001 年雖然全年實質 GDP 成長率為正，但 **「2001 年前三個季度（Q1、Q2、Q3）每一季的實質 GDP 成長率皆為負值」**，因此符合「連續至少兩季負成長」的衰退定義。
> - **最新論點 / 修正後數據（根據 [[source-blanchard-chap-5|Blanchard Ch.5 Slide 48–49]]）**：
>   - 根據美國 BEA 事後**修正後數據（Revised data, Figure A1）**，2001 年第 2 季（2001 Q2）的實質 GDP 成長率其實是**小幅正成長**（負成長季度為 2000 Q3、2001 Q1 與 2001 Q3，**並未出現連續兩季負成長**）！
> - **關鍵差異原因與結論**：
>   - 國民所得（GDP）初值公布後會隨完整普查資料回溯修正（呼應 Ch.2 提及之 BEA 資料修正機制）。儘管修正後未滿足「連續兩季負成長」的簡易法則，但 **NBER** 綜合考量全美就業人數、工業生產與實質所得後，仍正式認定美國在 **2001 年 3 月至 2001 年 12 月** 經歷了一次經濟衰退。

---

## 7. 關聯頁面與來源索引 (References)
- **延伸對比**：[[fixed-base-vs-chain-linked-gdp|實質 GDP 衡量對比：定基法 (Fixed-Base) vs. 連鎖法 (Chain-Linked)]]、[[cpi-vs-pce-vs-gdp-deflator|三大通膨與物價指標對比：CPI vs. PCE vs. GDP Deflator]]
- **相關概念**：[[goods-market-and-multiplier|商品市場均衡、凱因斯消費函數與乘數效果]]、[[unemployment-and-labor-market-indicators|失業率與勞動市場指標]]、[[inflation-and-price-indexes|通貨膨脹與物價指數]]、[[okuns-law-and-phillips-curve|歐肯法則與菲利浦曲線]]
- **引用來源**：[[source-blanchard-chap-2|Blanchard Ch.2]]、[[source-blanchard-chap-3|Blanchard Ch.3]]、[[source-blanchard-chap-5|Blanchard Ch.5]]
