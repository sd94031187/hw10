---
title: "Blanchard Ch.11：儲蓄、資本累積與產出 (Saving, Capital Accumulation, and Output)"
category: source
source_path: "../../raw/Chap-11.pdf"
source_date: 2026-11-16
author: "Olivier Blanchard (Macroeconomics, 8th Edition)"
tags:
  - source
  - macroeconomics
  - solow-model
  - steady-state
  - golden-rule
  - human-capital
  - behavioral-economics
created: 2026-11-16
updated: 2026-11-16
source_count: 1
status: active
---

# Blanchard Ch.11：儲蓄、資本累積與產出

- **原始檔案**：[Chap-11.pdf](../../raw/Chap-11.pdf)（共 61 頁，含課堂教授完整微積分推導筆記與勘誤）
- **核心主題**：完整建構無技術進步與無人口成長下的**索洛成長模型（Solow Growth Model）**，推導人均資本動態方程式與**穩態（Steady State）**，確立儲蓄率 $s$ 對長期水準與成長率的三大定理，推導最大化長期消費的**資本黃金法則（Golden Rule Level of Capital, $s_G = \alpha$）**，分析現收現付制社會安全制度（Pay-as-you-go Social Security）與行為經濟學「明天存更多（Save More Tomorrow）」計畫，最後將模型擴展至納入**人力資本（Human Capital, $H$）**。

---

## 1. Gate 1 前置驗算與重大印刷筆誤修正紀錄

> [!WARNING] Gate 1 重大公式印刷筆誤修正 (`Chap-11.pdf` p.61 附錄 Cobb-Douglas 穩態人均資本公式)
> - **原始投影片誤印（Slide 61）**：在附錄推導柯布—道格拉斯生產函數 $Y = K^\alpha N^{1-\alpha}$（即人均形式 $y = k^\alpha$）的穩態時，Slide 60 正確寫出穩態條件：
>   $$s\left(\frac{K^*}{N}\right)^\alpha = \delta\left(\frac{K^*}{N}\right) \implies \delta\left(\frac{K^*}{N}\right)^{1-\alpha} = s \implies \left(\frac{K^*}{N}\right)^{1-\alpha} = \frac{s}{\delta}$$
>   但到了 **Slide 61**，投影片卻將兩邊取 $\frac{1}{1-\alpha}$ 次方的結果誤印成多乘了一個 $\alpha$：
>   $$\text{Slide 61 誤印：}\quad \frac{K^*}{N} = \left(\frac{s}{\delta}\right)^{\frac{\alpha}{1-\alpha}} \quad \text{並宣稱「當 } \alpha = 0.5 \text{ 時，} \frac{K^*}{N} = \frac{s}{\delta}\text{」}$$
> - **Gate 1 獨立驗算與課堂手寫筆記核對**：
>   1. 對 $\left(\frac{K^*}{N}\right)^{1-\alpha} = \frac{s}{\delta}$ 兩邊取 $\frac{1}{1-\alpha}$ 次方，正確的**穩態人均資本（$k^* = K^*/N$）**與**穩態人均產出（$y^* = Y^*/N = (k^*)^\alpha$）**分別為：
>      $$\frac{K^*}{N} = \left(\frac{s}{\delta}\right)^{\frac{1}{1-\alpha}}, \qquad \frac{Y^*}{N} = \left(\frac{K^*}{N}\right)^\alpha = \left(\frac{s}{\delta}\right)^{\frac{\alpha}{1-\alpha}}$$
>   2. 當 $\alpha = 0.5$ 時，$\frac{1}{1-\alpha} = 2$ 且 $\frac{\alpha}{1-\alpha} = 1$，因此：
>      $$\frac{K^*}{N} = \left(\frac{s}{\delta}\right)^2, \qquad \frac{Y^*}{N} = \frac{s}{\delta}$$
>   3. 這完全印證了正文中 **Slides 40–41 的數值模擬**（設 $\alpha = 0.5, \delta = 10\%$：當 $s$ 從 $10\%$ 翻倍為 $20\%$ 時，穩態人均資本 $K^*/N$ 從 $\left(\frac{0.1}{0.1}\right)^2 = 1$ **暴增 4 倍為 $\left(\frac{0.2}{0.1}\right)^2 = 4$**，而穩態人均產出 $Y^*/N$ 則從 $1$ **翻倍為 $\sqrt{4} = 2$**）。課堂教授在 Slides 18、27、50 的手寫板書也明確寫出 $k^* = (s/\delta)^{\frac{1}{1-\alpha}}$ 與 $y^* = (s/\delta)^{\frac{\alpha}{1-\alpha}}$，確認 Slide 61 是把 $Y^*/N$ 的指數誤植到 $K^*/N$ 上！

---

## 2. 索洛模型核心方程式與穩態（Slides 2–17）

1. **基本假設**：
   - 人口與勞動力固定不變（$N_t = N$），且無技術進步（生產函數 $f(\cdot)$ 不隨時間改變）。
   - 封閉經濟且政府預算平衡（$T = G$），故投資恆等於私人儲蓄：
     $$I_t = S_t = s Y_t$$
   - 資本每年以固定折舊率 $\delta$ 損耗：
     $$K_{t+1} = (1 - \delta)K_t + I_t = (1 - \delta)K_t + s Y_t$$
2. **人均資本動態方程式（Law of Motion of Capital per Worker，Slides 9–11）**：
   將上式同除以 $N$ 並移項，得到人均資本變動量：
   $$\frac{K_{t+1}}{N} - \frac{K_t}{N} = s f\left(\frac{K_t}{N}\right) - \delta \frac{K_t}{N}$$
   - **經濟直覺**：$\text{人均資本變動} = \text{人均新增投資 } s f(k_t) - \text{人均資本折舊 } \delta k_t$。
     - 當 $s f(k_t) > \delta k_t$（新增投資大於折舊）：人均資本持續增加（$k_{t+1} > k_t$），經濟處於成長過渡期。
     - 當 $s f(k_t) < \delta k_t$（新增投資不足以彌補折舊）：人均資本萎縮（$k_{t+1} < k_t$）。
3. **穩態（Steady State，Slides 16–17）**：
   - 當人均資本與人均產出不再變動（$\Delta k = 0$）時，經濟達到長期均衡**穩態 $(K^*/N, Y^*/N)$**：
     $$s f\left(\frac{K^*}{N}\right) = \delta \left(\frac{K^*}{N}\right)$$
   - **歷史實證：二戰後法國的經濟奇蹟（1946–1950，Slides 14–15）**：二戰摧毀了法國約 $30\%$ 的資本存量（住宅、鐵路、橋樑、工廠），使戰後初期的 $K_0/N$ 遠低於穩態 $K^*/N$。根據索洛模型，當 $k_0 \ll k^*$ 時，新增投資遠大於折舊，經濟會經歷極高速的**過渡期追趕成長（Transitional Growth）**——法國在 1946–1950 年間實質 GDP 年均成長率高達 **$9.6\%$**（5 年內實質產出激增約 $58\%$）！

---

## 3. 儲蓄率（$s$）的三大黃金定理與黃金法則（Slides 18–52）

### 3.1 儲蓄率對經濟的三大影響（Slides 18–26）
1. **儲蓄率對「長期穩態成長率」毫無影響**：在沒有技術進步下，無論儲蓄率 $s$ 是 $10\%$ 還是 $40\%$，達到穩態後的長期人均產出成長率永遠等於 **$0\%$**。
2. **儲蓄率決定「長期穩態的人均產出水準（Level Effect）」**：較高的儲蓄率 $s_1 > s_0$ 會使穩態人均資本由 $K_0^*/N$ 上升至 $K_1^*/N$，穩態人均產出由 $Y_0^*/N$ 上升至 $Y_1^*/N$。
3. **提高儲蓄率會在「過渡期間（Transition）」創造暫時的正成長**：在從舊穩態邁向新穩態的數十年間（如 $\alpha = 0.5, \delta = 10\%$ 下，約需 10 年完成 $40\%$ 調整、20 年完成 $63\%$ 調整），經濟成長率會暫時大於零。

### 3.2 資本黃金法則（Golden Rule Level of Capital, $s_G$，Slides 27–37, 47–52）
- **核心問題**：如果提高儲蓄率可以推升穩態產出，政府應該把儲蓄率推到 $100\%$ 嗎？**絕對不行！** 因為人們最終關心的是**消費（Consumption, $C/N$）**，而非產出本身（若 $s=1$，所有產出都拿去造機器修機器，$C=0$，國民會餓死）。
- **穩態人均消費方程式（Slide 29）**：
  $$\frac{C^*}{N} = \frac{Y^*}{N} - \delta \frac{K^*}{N} = f\left(\frac{K^*}{N}\right) - \delta \frac{K^*}{N}$$
- **黃金法則條件（課堂手寫微積分推導，Slides 27, 29, 50）**：
  對 $C^*/N$ 關於 $k^* = K^*/N$ 微分並令其為 $0$：
  $$\frac{d(C^*/N)}{dk^*} = f'(k_G^*) - \delta = 0 \implies \mathbf{f'(k_G^*) = \delta} \quad (\text{資本邊際產出 } MPK = \text{折舊率 } \delta)$$
  在柯布—道格拉斯生產函數 $y = k^\alpha$ 下：
  $$c^* = (1 - s)\left(\frac{s}{\delta}\right)^{\frac{\alpha}{1-\alpha}}$$
  取對數微分求極大值：
  $$\frac{d \ln c^*}{ds} = -\frac{1}{1-s} + \frac{\alpha}{1-\alpha}\frac{1}{s} = 0 \implies \mathbf{s_G = \alpha}$$
  - 在教科書數值模擬（$\alpha = 0.5, \delta = 10\%$，Slide 47 Table 11.1）中，黃金法則儲蓄率為 **$s_G = 50\%$**（此時 $K^*/N = 25, Y^*/N = 5.0, C^*/N = 2.5$ 達到最高）。
- **兩種偏離黃金法則的政策取捨（Slides 31–37）**：
  - **動態無效率（Dynamic Inefficiency，$s > s_G$）**：儲蓄過度！此時調降儲蓄率不僅能**立即增加當代消費**，連**未來穩態消費也會一起上升**（雙贏，無跨代取捨）。
  - **儲蓄不足（$s < s_G$，現實中絕大多數 OECD 國家皆屬此類，如美國總儲蓄率約 $17\%$、家庭儲蓄率僅約 $6\%$）**：提高儲蓄率雖能提高未來子孫的穩態消費，但**當代人必須先忍受消費下降的犧牲**（跨代取捨 Intergenerational Trade-off）。由於未來世代沒有投票權，加上**現收現付制（Pay-as-you-go）社會安全退休金**降低了年輕人自己存錢養老的誘因，導致各國儲蓄率長期偏低。
  - **行為經濟學解方（Slide 35）**：諾貝爾獎得主 Richard Thaler 與 Shlomo Benartzi 設計的 **「明天存更多（Save More Tomorrow）」** 計畫，讓員工預先承諾將「未來加薪幅度的一部分」自動轉入退休儲蓄，克服人性短視與損失規避，使參與者儲蓄率在 4 次加薪後從 $3.5\%$ 躍升至 $13.6\%$。

---

## 4. 實體資本 vs. 人力資本（Physical vs. Human Capital，Slides 53–59）

- **擴充生產函數**：
  $$\frac{Y}{N} = f\left(\frac{K}{N}, \frac{H}{N}\right)$$
  其中 $H/N$ 為**人均人力資本（Human Capital per Worker）**，由正規教育（Education）與在職訓練（On-the-job training）累積而成。
- **美國資本投入規模比較（Slide 56）**：美國花在正規高等與基礎教育的支出約佔 GDP 的 $6.5\%$（若計入學生放棄工作的機會成本與在職訓練則更高），與實體資本投資佔 GDP 比例（約 $16\%$）屬於同一量級。
- **內生成長理論延伸（Endogenous Growth Models，課堂手寫筆記 Slides 36, 53）**：課堂教授特別補充，若納入知識研發（R&D）與人力資本 $H$，廣義資本可能不再受限於邊際報酬遞減（甚至呈現報酬遞增），這正是內生成長理論解釋長期持續成長的關鍵切入點。

---

## 5. 關聯 Wiki 頁面

- `[[solow-growth-model-and-golden-rule|索洛成長模型 (Solow Model)、穩態與黃金法則儲蓄率]]`
- `[[economic-growth-ppp-and-happiness|長期經濟成長事實：購買力平價 (PPP)、快樂經濟學與跨國收斂]]`
- `[[saving-short-run-paradox-vs-long-run-growth|儲蓄的跨期大對決：短期節儉矛盾 vs. 長期索洛資本累積與黃金法則]]`
- `[[goods-market-and-keynesian-multiplier|商品市場均衡、凱因斯乘數與節儉矛盾]]`
