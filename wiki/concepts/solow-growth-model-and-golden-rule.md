---
title: "索洛成長模型 (Solow Model)、穩態與黃金法則儲蓄率 (Steady State & Golden Rule)"
category: concept
tags:
  - macroeconomics
  - solow-model
  - steady-state
  - golden-rule
  - capital-accumulation
  - human-capital
created: 2026-11-16
updated: 2026-11-16
source_count: 2
status: active
---

# 索洛成長模型 (Solow Model)、穩態與黃金法則儲蓄率

## 1. 核心架構：總體生產函數與資本累積引擎

諾貝爾經濟學獎得主 Robert Solow 提出的**索洛成長模型（Solow Growth Model）**是所有現代長期經濟成長分析的基石。

### 1.1 總體生產函數的兩大性質（`[[source-blanchard-chap-10]]`）
設總產出 $Y = F(K, N)$，具備：
1. **規模報酬固定（Constant Returns to Scale, CRTS）**：工廠、機器（$K$）與勞工（$N$）同時翻倍，產出（$Y$）也剛好翻倍。將方程式同除以勞動人數 $N$，即可得到**人均產出（$Y/N$）僅取決於人均資本（$K/N$）**的關係：
   $$\frac{Y}{N} = f\left(\frac{K}{N}\right)$$
2. **資本邊際報酬遞減（Decreasing Returns to Capital）**：當每位員工已經有 1 台電腦時，再給他第 2 台、第 3 台電腦，所能增加的產出越來越少（$f(K/N)$ 曲線向上彎曲但越來越平緩）。

### 1.2 人均資本動態方程式（Law of Motion of Capital，`[[source-blanchard-chap-11]]`）
在封閉且預算平衡的經濟體中，儲蓄等於投資（$I = S = sY$），而現有機器設備每年有固定比例 $\delta$ 會損壞折舊。因此，明年的「人均資本變動量」等於**「人均新增投資」減去「人均資本折舊」**：

$$\frac{K_{t+1}}{N} - \frac{K_t}{N} = s f\left(\frac{K_t}{N}\right) - \delta \frac{K_t}{N}$$

---

## 2. 長期穩態（Steady State）與儲蓄率的三大黃金定理

因為新增投資曲線 $s f(K/N)$ 會隨資本增加而邊際遞減（越來越平緩），但折舊直線 $\delta (K/N)$ 卻按固定比例一路向上，兩條線最終必定相交於一點——此時**新增投資剛好只夠修補壞掉的折舊機器（$\Delta (K/N) = 0$）**，經濟進入**穩態（Steady State, $K^*/N$ 與 $Y^*/N$）**：

$$s f\left(\frac{K^*}{N}\right) = \delta \left(\frac{K^*}{N}\right)$$

> [!WARNING] Gate 1 重大公式印刷筆誤修正 (`Chap-11.pdf` p.61)
> 在柯布—道格拉斯生產函數 $Y = K^\alpha N^{1-\alpha}$（即 $Y/N = (K/N)^\alpha$）下，由 $s(K^*/N)^\alpha = \delta(K^*/N)$ 求解穩態：
> - **正確公式（經 Gate 1 驗算與課堂手寫板書確認）**：
>   $$\text{穩態人均資本：}\frac{K^*}{N} = \left(\frac{s}{\delta}\right)^{\frac{1}{1-\alpha}}, \qquad \text{穩態人均產出：}\frac{Y^*}{N} = \left(\frac{s}{\delta}\right)^{\frac{\alpha}{1-\alpha}}$$
> - **原始投影片 p.61 筆誤**：誤將 $K^*/N$ 印成 $(s/\delta)^{\frac{\alpha}{1-\alpha}}$。當 $\alpha = 0.5$ 時，正確的 $K^*/N = (s/\delta)^2$（儲蓄率翻倍會使穩態資本變 **4 倍**、穩態產出變 **2 倍**，如投影片 p.40–41 所示）。

### 儲蓄率（$s$）的三大核心定理
1. **儲蓄率無法改變「長期成長率」**：在沒有技術進步的情況下，無論儲蓄率多高，長期穩態的人均成長率永遠是 **$0\%$**。
2. **儲蓄率決定「長期富裕水準（Level Effect）」**：儲蓄率越高的國家，穩態的人均資本 $K^*/N$ 與人均產出 $Y^*/N$ 水準越高。
3. **提高儲蓄率（或戰後重建）會帶來「過渡期的高成長（Transitional Growth）」**：例如**二戰後法國（1946–1950）**因戰爭摧毀了 $30\%$ 資本存量（$K_0/N \ll K^*/N$），新增投資遠大於折舊，使其在戰後 5 年內創下年均 **$9.6\%$** 的驚人追趕成長率！

---

## 3. 存越多錢越好嗎？資本黃金法則（Golden Rule Level of Capital, $s_G$）

如果提高儲蓄率能讓穩態產出變高，那國家應該規定大家把 $100\%$ 的收入都存起來買機器（$s = 100\%$）嗎？
- **絕對不行！** 因為人們工作的目的是為了**消費（吃美食、旅遊、住好房，$C/N$）**，而不是為了看工廠裡堆滿機器。
  - 若 $s = 0\%$：沒有機器，產出為 $0$，消費 $C^*/N = 0$。
  - 若 $s = 100\%$：所有產出全部拿去買機器和修補折舊機器，留給人民的消費也是 $C^*/N = 0$！
- **黃金法則儲蓄率（$s_G$）**：能讓**長期穩態人均消費 $C^*/N = f(K^*/N) - \delta(K^*/N)$ 達到最高峰**的儲蓄率。
  - 數學條件：當**資本邊際產出等於折舊率（$MPK = f'(k_G^*) = \delta$）**時，穩態消費最大。在 $Y = K^\alpha N^{1-\alpha}$ 下，黃金法則儲蓄率剛好等於資本所得份額 **$s_G = \alpha$**（例如當 $\alpha = 0.5, \delta = 10\%$ 時，$s_G = 50\%$）。

| 儲蓄率區間 | 經濟狀態 | 政策調整的跨代影響（Intergenerational Effect） |
| :--- | :--- | :--- |
| **$s > s_G$**<br>（儲蓄過度） | **動態無效率（Dynamic Inefficiency）**<br>（機器多到修機器的折舊成本大於新機器產出） | **雙贏（無痛改革）**：調降儲蓄率，不僅當代人可以立刻多消費，未來子孫的穩態消費也會一起增加！ |
| **$s < s_G$**<br>（儲蓄不足，如美國 $s \approx 17\%$） | **常態經濟體**<br>（低於黃金法則） | **跨代兩難取捨**：若要提高儲蓄率讓未來子孫享有更高消費，**當代人必須先勒緊褲帶、忍受數十年消費下降的犧牲**。 |

- **行為經濟學如何幫現代人多存錢？** 諾貝爾獎得主 Richard Thaler 推出 **「明天存更多（Save More Tomorrow）」** 方案——不要求員工現在減薪存錢，而是簽約同意「未來每次加薪時，自動把加薪的一部分撥入退休金」，短短 4 次加薪就讓員工儲蓄率從 $3.5\%$ 暴增至 $13.6\%$！

---

## 4. 廣義資本：實體資本（$K$）與人力資本（$H$）

除了廠房與機器（實體資本 $K$），勞動者的知識、教育與技能則是**人力資本（Human Capital, $H$）**：
$$\frac{Y}{N} = f\left(\frac{K}{N}, \frac{H}{N}\right)$$
- 一國的長期富裕水準，同時取決於**「物質儲蓄率 $s_K$」**與**「教育與培訓投入率 $s_H$」**。
- 當我們把科學研發（R&D）與知識累積納入廣義人力資本時，因為「知識可以重複共享且啟發新點子」，可能打破邊際報酬遞減的魔咒，成為推動長期持續成長的**內生成長（Endogenous Growth）**引擎。

---

## 5. 關聯頁面與來源

- **原始教材來源**：
  - `[[source-blanchard-chap-11|Blanchard Ch.11：儲蓄、資本累積與產出]]`
  - `[[source-blanchard-chap-10|Blanchard Ch.10：經濟成長的事實 (The Facts of Growth)]]`
- **概念與延伸連結**：
  - `[[economic-growth-ppp-and-happiness|長期經濟成長事實：購買力平價 (PPP)、快樂經濟學與跨國收斂]]`
  - `[[saving-short-run-paradox-vs-long-run-growth|儲蓄的跨期大對決：短期節儉矛盾 vs. 長期索洛資本累積與黃金法則]]`
  - `[[goods-market-and-keynesian-multiplier|商品市場均衡、凱因斯乘數與節儉矛盾]]`
