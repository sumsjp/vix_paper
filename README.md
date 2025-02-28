A. [Quantitative](#A)<br>
B. [Arbitrage](#B)<br>
C. [Volatility Risk Premium](#C)<br>
D. [Machine Learning](#D)<br>
E. [Market Study](#E)<br>

---

<a name="A"></a>
A. Quantitative

---

<a name="B"></a>
B. Arbitrage

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

---

<a name="C"></a>
C. Volatility Risk Premium

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

[[中文]](chn/[08]Harvesting_VRP.md) [[英文]](eng/[08]Shibo_Lu_01210524.pdf)
</details>
<!-- #endregion -->

---

<a name="D"></a>
D. Machine Learning

<!-- #region D1 -->
<details>
<summary>1. (2024) VIX Constant Maturity Futures Trading Strategy: A Walk-Forward Machine Learning Study</summary><br>

本研究利用**七種先進的機器學習方法**，針對 **VIX 恒定期限期貨（VIX CMFs）** 之次日收益進行數值預測，並基於預測結果提出一種新的 **約束均值方差投資組合優化策略（C-MVO）**，與傳統的**多空交易策略**進行比較，以評估機器學習預測的可行性與盈利能力。

本研究使用**三種特徵集**（包含 VIX CMFs 期限結構特徵），分別評估七種機器學習模型的預測能力與回測表現。在 **11 年的數據測試期間**，採用嚴格的 **walk-forward 擴展窗口方法** 進行訓練與回測。結果顯示：
1. **四種機器學習模型的預測信息比率（Information Ratio）大於 0.02，平均達 0.037**，表明 VIX CMFs 期限結構具有預測次日收益的能力。
2. **C-MVO 策略的平均信息比率為 0.623，顯著優於基準多空策略的 0.404**，證明機器學習預測結果可有效提升交易績效。
3. **線性回歸模型（Linear Regression）在預測與回測表現上優於所有其他機器學習模型**，顯示 VIX 期貨期限結構特徵與次日收益呈較線性的關係，而過於複雜的非線性模型可能導致過擬合。
4. **統計衍生特徵對預測能力的提升有限**，顯示期限結構本身已包含關鍵資訊。

本研究證明 **VIX CMFs 期限結構可作為有效的交易信號**，並提供了一種基於機器學習的 VIX 期貨交易策略，為量化交易與風險管理提供新的方法論與應用方向。未來研究可進一步探索**高頻數據**與**更先進的深度學習模型**，以提升預測準確性與交易策略的盈利能力。

[[中文]](chn/[09]VIX_CMFS_CMVO.md) [[英文]](eng/[09]VIX_constant_maturity_futures_trading_strategy_A_w.pdf)
</details>
<!-- #endregion -->

<!-- #region D2 -->
<details>
<summary>2. (2022) Trading Signals in VIX Futures</summary><br>

本研究提出了一種基於深度學習的VIX期貨交易策略，假設VIX期貨的期限結構遵循馬爾可夫模型，並透過深度神經網絡（DNN）來選擇最優交易信號，以最大化日內預期效用。我們利用歷史VIX期貨數據進行回測，結果顯示該方法能夠在不同市場環境下提供有效的交易信號，並在無交易成本的情境下展現出顯著的投資組合收益與高Sharpe比率。

研究發現，VIX期貨的期限結構通常呈現順價（Contango），而當市場進入反向市場（Backwardation）時，交易信號能夠動態調整部位，以捕捉市場回歸趨勢來獲利。此外，透過k折交叉驗證，我們驗證了神經網絡能夠有效學習VIX期貨曲線的關鍵特徵，並產生穩健的交易信號。然而，當考慮交易成本後，策略的收益有所下降，顯示實務操作需謹慎考量成本因素。

本研究證明了深度學習技術在VIX期貨交易中的應用潛力，並為基於期限結構的交易策略提供了一種數據驅動的方法。然而，由於交易信號可能伴隨較高的最大回撤（Maximum Drawdown），未來應進一步探索更嚴格的風險管理策略及優化模型，以提升實際應用的可行性。

[[中文]](chn/[10]Trading_Signals_VIX.md) [[英文]](eng/[10]2103.02016v3.pdf)
</details>
<!-- #endregion -->

<!-- #region D3 -->
<details>
<summary>3. (2021) The VIX Index under Scrutiny of Machine Learning Techniques and Neural Networks</summary><br>

本研究探討 **芝加哥期權交易所（CBOE）波動率指數（VIX）** 的計算方法，並利用機器學習與深度學習技術（如神經網絡與長短期記憶網絡 LSTM）來複製和預測 VIX 指數及其期貨。VIX 指數基於 S&P 500 選擇權市場報價計算，然而，其受少數選擇權價格影響，存在市場操縱的可能性。研究結果顯示，**無需使用 CBOE 方法選定的所有選擇權（約 300 個），僅使用 52 個關鍵選擇權便可準確複製 VIX 指數**，並透過神經網絡學習其計算公式。

基於基本神經網絡與 LSTM 模型，我們發現：
1. **VIX 指數可以透過較少數量的選擇權複製**，並且神經網絡能成功學習 VIX 的計算方式，預測效果良好。
2. **LSTM 多層模型在 VIX 指數的預測上表現最佳**，能有效學習市場長期依賴關係。
3. **VIX 期貨的預測準確度較低**，即使使用相同的深度學習方法，預測誤差仍然較大。
4. **研究結果揭示 VIX 可能受少數選擇權影響，這可能導致套利機會或市場操縱的可能性**。

[[中文]](chn/[11]VIX_Scrutiny_NN.md) [[英文]](eng/[11]2102.02119v1.pdf)
</details>
<!-- #endregion -->

---

<a name="E"></a>
E. Market Study

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

<!-- #region E3 -->
<details>
<summary>3. (2023) Media Coverage of Market Volatility and the Information Content for VIX Trading</summary><br>

本研究透過文本分析方法衡量媒體情緒，主要分析新聞報導、博客文章及討論訊息，以探討其與市場情緒的關聯性，特別是對VIX期貨回報的影響。本研究發現，基於媒體情緒指數（隔夜計算），可以有效預測每日VIX期貨回報。然而，宏觀經濟公告會削弱其預測能力。此外，當發文量較大、交易量高、波動性增強及市場流動性較低時，情緒效應更為顯著。

透過媒體情緒指數的交易策略顯示，該策略具有較高的績效，特別是基於新聞文章的分析結果最為顯著。這些結果表明，媒體情緒在波動性交易中具有經濟價值。

[[中文]](chn/[11]Media-Coverage-of-Market-Volatility.md) [[英文]](eng/[11]Media-Coverage-of-Market-Volatility.docx_20230704.pdf)
</details>
<!-- #endregion -->

<!-- #region E4 -->
<details>
<summary>4. (2018) Is the VIX a Reliable Indicator of Stock Market Volatility?</summary><br>

本論文探討芝加哥期權交易所波動率指數（VIX）作為股市波動性指標的可靠性。VIX 被廣泛稱為市場的「恐慌指數」，其計算基於 S&P 500 指數期權價格，反映市場對未來 30 天內波動的預期。本研究使用 GARCH（1,1）模型，將 VIX 的變動與市場指數的日內波動範圍（市場實現波動性）進行實證分析。

研究結果顯示：
1. **VIX 與市場波動性**：VIX 的變動與 S&P 500 指數的市場波動範圍之間存在顯著的正向關係，表明 VIX 確實能夠有效衡量市場的即時波動性。
2. **VIX 的不對稱影響**：VIX 上升時對市場波動範圍的影響大於下降時的影響，這與行為財務學中的前景理論相符，顯示市場對風險的反應具有不對稱性。
3. **交易時段的影響**：VIX 在非交易時段（夜間）的變動能夠預測未來四天的市場波動，而交易時段內的 VIX 變動則對市場波動的影響可持續五天，並且影響力隨時間減弱。
4. **週期效應**：VIX 在星期五的變動對市場波動範圍的影響最強，這可能與週末即將到來的不確定性（如財報發布、政策變動等）有關，而週三的市場波動則相對較低。

本研究的結果證實，VIX 是衡量市場波動性的重要指標，投資者應關注 VIX 的變動，特別是在不同交易時段和不同交易日的影響。此外，本研究建議市場參與者在分析 VIX 影響時，應區分交易時段與非交易時段的變動，以獲得更準確的市場波動預測。未來研究可進一步探討 VIX 在不同市場環境（如經濟週期或政策變動）下的行為特徵。

[[中文]](chn/[12]VIX_Indicator_Stock_Market.md) [[英文]](eng/[12]EZEONYEKA-THESIS-2018.pdf)
</details>
<!-- #endregion -->


---

<!-- #region X0 -->
<details>
<summary></summary><br>

[[中文]](chn) [[英文]](eng)
</details>
<!-- #endregion -->
