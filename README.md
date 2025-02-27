A. [Quantitative](#A)<br>
B. [Arbitrage](#B)<br>
C. [Volatility Risk Premium](#C)<br>
D. [Machine Learning](#D)<br>
E. [Market Study](#E)<br>

---

<a name="A"></a>
A. Quantitative

<!-- #region Quantitative -->

<!-- #region A1 -->

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

<a name="B"></a>
B. Arbitrage

<!-- #region Arbitrage -->
<!-- #region B1 -->

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

<!-- #region B2 -->

<details>
<summary>2. (2020) The Law of One Price in Equity Volatility Markets</summary><br>

本研究探討股權波動率市場中 **單一價格法則（Law of One Price）** 的違反現象。雖然 VIX 期貨價格理論上應受無套利限制，但實證結果顯示其價格經常顯著偏離由標普 500 指數期權隱含的上限。這種偏差在市場壓力時期（如金融危機或市場大幅波動時）尤為明顯。

研究發現，這些價格偏差不僅代表靜態套利機會，且具有 **顯著的回報預測能力** 。基於價格偏差構建的 **相對價值交易策略** ，即在期貨價格高於上限時做空、低於下限時做多，能夠獲得高 Sharpe 比率並實現經濟上顯著的超額回報。

進一步分析顯示， **系統性風險與市場需求壓力** 對套利偏差有重要影響。當市場風險上升時，VIX 期貨價格對風險變動的反應小於標普 500 指數期權價格，導致套利偏差縮小。此外，來自散戶與對沖基金的需求壓力（如 VIX 交易所交易產品的影響）亦可能推動 VIX 期貨價格偏離其理論價值。

本研究的結果表明，VIX 期貨與標普 500 指數期權市場之間的套利違規現象廣泛且持續存在，這對投資者和政策制定者在解讀市場風險指標時提出了挑戰，並突顯了市場摩擦對資產定價的影響。

[[中文]](chn/[05]law_price_in_equity_volatility.md) [[英文]](eng/[05]sr953.pdf)
</details>

<!-- #endregion -->

<!-- #endregion -->

---

<a name="C"></a>
C. Volatility Risk Premium

<!-- #region Volatility Risk Premium -->

<!-- #region C1 -->

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

<!-- #region C2 -->
<details>
<summary>2. (2020) Selling VIX Futures and Options for Portfolio Return Enhancement</summary><br>

本研究探討**賣出VIX期貨與選擇權策略**對於**投資組合回報增強（Return Enhancement）**的影響，並評估其風險與回報特性。由於VIX期貨期限結構多呈順價差（Contango），賣出VIX期貨策略可能在某些市場環境下產生異常優異的表現。然而，該策略亦存在極端的尾部風險，特別是在市場波動劇增的時期，如**2008年金融危機**與**2018年2月「波動性風暴（Volmageddon）」**。

研究發現，小額配置於VIX賣出策略可提高投資組合回報，但裸賣VIX部位可能導致潛在的經濟災難性損失。為降低風險，研究分析了**動態槓桿調整策略（Dynamic De-levering Strategies）**，如**VPDSM與VPNSM指數**，透過調整槓桿比例與VIX買權對沖，降低波動性與最大回撤，提升風險調整後回報。

研究結果顯示，VIX賣出策略在市場穩定時可提升投資組合回報並擴展**效率前緣（Efficient Frontier）**，但長期持有或過度配置可能導致重大虧損。投資者應謹慎管理槓桿與風險對沖，以降低極端市場情境下的損失風險。

[[中文]](chn/[07]Selling_VIX_Futures_and_Options.md) [[英文]](eng/[07]Szado_Selling_VIX_Fut_&_Opt_for_Enhancement_June_15_2020.pdf)
</details>
<!-- #endregion -->

<!-- #region C3 -->
<details>
<summary>3. (2020) Harvesting Volatility Risk Premium
</summary><br>

本研究探討**波動率風險溢酬 (Volatility Risk Premium, VRP)** 的提取方式，特別關注**賣出 delta 對沖期權 (delta-hedged options)** 與**波動率互換 (variance swaps)** 兩種策略在不同金融模型下的表現。透過理論推導與數值模擬，研究發現：

1. **VRP 來源於隱含波動率高於實現波動率的現象**，市場參與者可透過賣出波動率相關產品來獲取收益。
2. **在 Black-Scholes 模型下，delta 對沖期權策略可有效提取 VRP**，但當市場存在**隨機波動率 (Heston 模型)** 或**跳躍風險 (Merton 模型)** 時，該策略的風險顯著增加，甚至可能產生極端虧損。
3. **波動率互換 (variance swaps) 在隨機波動率與跳躍市場下提供更穩定的 VRP 提取方式**，能較有效對沖市場風險。
4. **在隨機波動率與跳躍市場 (Stochastic Volatility Jump Diffusion, SVJD) 下，單純依賴 delta 對沖期權無法有效提取 VRP，甚至可能造成重大損失**，因此需要動態調整交易策略。

[[中文]](chn) [[英文]](eng)
</details>
<!-- #endregion -->

<!-- #endregion -->

---

<a name="D"></a>
D. Machine Learning

<!-- #region Machine Learning -->
<!-- #endregion -->

---

<a name="E"></a>
E. Market Study

<!-- #region Market Study -->

<!-- #region E1 -->
<details>
<summary>1. (2020) Volatility Markets Underreacted to the Early Stages of the COVID-19 Pandemic</summary><br>

本研究探討 2020 年 COVID-19 疫情爆發初期，市場對風險的反應是否符合標準資產定價模型的預期。研究發現，VIX 期貨市場在疫情初期對不斷上升的風險反應不足，呈現「低溢價反應」現象。

這項研究為投資者提供了對市場非理性反應的深刻見解，並強調在極端市場條件下，利用 VIX 溢價異常信號進行交易的潛在獲利機會。

[[中文]](chn/[02]VIX_Underreacted_COVID-19.md) [[英文]](eng/[02]raaa010.pdf)
</details>

<!-- #endregion -->

<!-- #region E2 -->
<details>
<summary>2. (2020) Time-Dependent Lead-Lag Relationships between the VIX and VIX Futures Markets</summary><br>

本研究利用**對稱熱最優路徑方法（Symmetric Thermal Optimal Path, TOPS）**，探討**VIX（波動率指數）與 VIX 期貨市場**之間的動態交互模式。研究發現：

1. 在最初幾年，尤其是在**VIX 期權推出之前**，VIX 指數對 VIX 期貨的影響較為顯著，顯示出 VIX 主導 VIX 期貨市場的情況。
2. 通過 TOPS 方法分析的領先-滯後關係顯示，VIX 與 VIX 期貨之間的關係並非固定不變，而是呈現**交替變化的模式**，而非單向的市場主導關係。
3. **VIX 期貨市場在價格發現中的作用隨時間增強**，特別是在**VIX 交易所交易產品（ETPs）推出後**，VIX 期貨市場變得更加重要。

本研究的發現對於理解 VIX 及其衍生產品在價格發現過程中的角色具有重要意義。

[[中文]](chn/[06]Time_Lead-Lag_VIX.md) [[英文]](eng/[06]1910.13729v1.pdf)
</details>
<!-- #endregion -->

<!-- #endregion -->

<!-- #endregion -->

---

<!-- #region X0 -->
<details>
<summary></summary><br>

[[中文]](chn) [[英文]](eng)
</details>
<!-- #endregion -->
