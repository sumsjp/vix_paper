A. [Trend Following](#A)<br>
B. [Mean Reversion](#B)<br>
C. [Arbitrage](#C)<br>
D. [Volatility Risk Premium](#D)<br>
E. [Machine Learning](#E)<br>
F. [Market Study](#F)<br>

---

<a name="A"></a>
A. Trend-Following

<!-- #region Trend Following -->
<!-- #endregion -->

---

<a name="B"></a>
B. Mean Reversion


<!-- #region Mean Reversion -->

<!-- #region B1 -->

<details>
<summary>1. (2016) Trading VIX Futures under Mean Reversion with Regime Switching</summary><br>

本研究探討了一種基於**均值回歸與狀態轉換（Regime Switching）**的最優VIX期貨交易策略。透過**Cox-Ingersoll-Ross（CIR）模型**並引入狀態轉換機制，我們建立了一個數學框架來分析投資者的最佳進場與退場時機。這涉及到求解**變分不等式（Variational Inequalities）**系統，以確定最佳交易邊界。

研究的核心內容包括：
1. **交易策略建模**：VIX 被建模為隨市場狀態變動的均值回歸過程，投資者可選擇**做多-平倉（long-short）或做空-平倉（short-long）**兩種交易策略。
2. **最優時機決策**：投資者在不同市場狀態下選擇進場、持倉或離場的最優決策，該決策受交易成本與市場狀態轉換影響。
3. **數值求解方法**：我們使用**投影逐次超鬆弛法（PSOR）**與Crank-Nicolson差分格式來求解最優停止問題，從而獲得最優交易邊界。
4. **交易邊界與市場狀態的影響**：研究發現，交易成本的存在會擴大投資者的等待區間（即更傾向於等待更好的價格）；此外，市場狀態的轉變會顯著影響交易策略，投資者應根據市場環境調整其進場與退場時機。

研究結果表明，在允許市場狀態轉換的情況下，投資者應**延遲進場，以獲取更優的交易機會**，相較於預先決定的單一做多或做空策略更具優勢。此外，本方法亦可應用於其他衍生性金融產品的最優交易決策，如**掉期（swaps）或期權（options）**。

[[中文]](chn/[01]Mean_Reversion_Regime_Switching.md) [[英文]](eng/[01]1605.07945v2.pdf)
</details>

<!-- #endregion -->

<!-- #endregion -->

---

<a name="C"></a>
C. Arbitrage

<!-- #region Arbitrage -->
<!-- #region C1 -->

<details>
<summary>1. (2017) Portfolio Effects of VIX Futures Index</summary><br>

本研究探討 **VIX 期貨指數** 作為**對沖工具**與**安全港資產**的有效性，分析其與 **S&P 500 指數** 之間的動態關係。研究涵蓋 **2006 年 1 月至 2016 年 7 月**，並採用 **GARCH 動態條件相關（DCC-GARCH）模型** 來檢測 VIX 期貨的避險特性。此外，我們通過回歸分析檢測 VIX 期貨在**極端市場波動**（股市下跌 10%、5%、1%）與**重大市場危機**（2008 年全球金融危機、2011 年美國信用評級下調、2016 年英國脫歐）期間的表現。

**研究結果顯示**：
1. **避險功能（Hedging）**：短期 VIX 期貨（STVIX）與中期 VIX 期貨（MTVIX）皆與 S&P 500 指數顯著負相關，證明其避險效果，中期 VIX 期貨表現更穩定。
2. **安全港特性（Safe Haven）**：VIX 期貨在股市極端下跌（10% 和 1% 分位數）時表現為**強安全港**，但在 5% 分位數時避險效果較弱。
3. **市場危機期間表現**：在**2008 年金融危機、2011 年信用評級下調與 2016 年英國脫歐**等事件期間，VIX 期貨表現為**強安全港資產**，且中期 VIX 期貨的避險效果優於短期 VIX 期貨。
4. **投資組合影響**：短期 VIX 期貨可能降低投資組合的長期回報，而中期 VIX 期貨對投資組合的影響較為中性，顯示較高的風險調整後回報（Sharpe Ratio）。

**結論**：本研究證明 VIX 期貨具有穩定的避險功能，特別是在市場動盪期間可作為**安全港資產**。然而，**長期持有 VIX 期貨可能產生負回報**，投資者應透過**動態交易策略**來優化投資組合配置，避免單純的「買入並持有」策略。

[[中文]](chn/[03]Portfolio_Effects_VIX.md) [[英文]](eng/[03]Portfolio_Effects_of_VIX_Futures_Index.pdf)
</details>

<!-- #endregion -->
<!-- #endregion -->

---

<a name="D"></a>
D. Volatility Risk Premium

<!-- #region Volatility Risk Premium -->

<!-- #region D1 -->

<details>
<summary>1. (2014) The VIX Futures Basis: Evidence and Trading Strategies</summary><br>

1. **基差無法有效預測 VIX 指數變動**  
2. **基差可用於預測 VIX 期貨回報**  
3. **基於基差的交易策略可獲利**  
4. **市場風險對沖與風險管理措施的影響**  

VIX 期貨基差主要反映 **波動率風險溢價（volatility risk premium）**，而非 VIX 指數的均值回歸特性。  
透過適當的交易策略與對沖，投資者可有效捕捉這一風險溢價，獲得穩健回報。本研究提供了新的實證證據，支持基於 VIX 期貨基差的套利策略。

[[中文]](chn/[04]VIX_Basis_Evidence_Tradin.md) [[英文]](eng/[04]The%20VIX%20Futures%20Basis_%20Evidence%20and%20Trading%20Strategies.pdf)
</details>

<!-- #endregion -->

<!-- #endregion -->

---

<a name="E"></a>
E. Machine Learning

<!-- #region Machine Learning -->
<!-- #endregion -->

---

<a name="F"></a>
F. Market Study

<!-- #region Market Study -->

<!-- #region F1 -->

<details>
<summary>1. (2020) Volatility Markets Underreacted to the Early Stages of the COVID-19 Pandemic</summary><br>

本研究探討 2020 年 COVID-19 疫情爆發初期，市場對風險的反應是否符合標準資產定價模型的預期。研究發現，VIX 期貨市場在疫情初期對不斷上升的風險反應不足，呈現「低溢價反應」現象。

這項研究為投資者提供了對市場非理性反應的深刻見解，並強調在極端市場條件下，利用 VIX 溢價異常信號進行交易的潛在獲利機會。

[[中文]](chn/[02]VIX_Underreacted_COVID-19.md) [[英文]](eng/[02]raaa010.pdf)
</details>

<!-- #endregion -->

<!-- #endregion -->

---

<!-- #region X0 -->

<details>
<summary></summary><br>

[[中文]](chn) [[英文]](eng)
</details>

<!-- #endregion -->
