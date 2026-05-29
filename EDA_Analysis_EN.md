# Crowding in ARP Strategies: Key Findings

## 1. NAV and Portfolio Overview
This analysis is based on two fund indices sharing the exact same 74 underlying instruments, serving as a perfect "natural experiment" to observe market consensus and divergence. Both indices frequently shift exposures between net long and short, confirming their nature as active, dynamic quantitative strategies.

![NAV Performance](./eda_figures/fig_1.png)
![Portfolio Composition](./eda_figures/fig_2.png)

## 2. Systemic Resonance in Crowding
Despite varying individual asset weights, the **portfolio concentration (HHI) of both strategies moves in complete tandem**, indicating that different quantitative models react uniformly to market opportunities and shocks (the root of systemic crowding). Due to high strategic homogeneity, we successfully captured **"Crowded Unwind" events** characterized by spikes in turnover and sudden drops in portfolio similarity.

![Crowding Metrics](./eda_figures/fig_3.png)
![Sector Heatmap](./eda_figures/fig_4.png)
![Daily Turnover](./eda_figures/fig_5.png)

## 3. Predictive Signals and Asset Divergence
Initial scatter plots verify that abrupt shifts in crowding metrics correlate with next-day return volatility. At the asset level, Equities and Rates represent high-consensus sectors prone to crowding, while Fixed Income and Commodities exhibit high model divergence.

![Returns vs Crowding](./eda_figures/fig_6.png)
![Top Crowded and Divergent Assets](./eda_figures/fig_7.png)

## 4. Next Steps
- **Factor Decomposition**: Map instruments to ARP factor tags (e.g., Momentum, Carry) to compute refined factor-level crowding.
- **Predictive Modeling**: Incorporate macro variables (VIX, Treasury yields) to perform long-term regression forecasts on drawdowns and tail risks.
