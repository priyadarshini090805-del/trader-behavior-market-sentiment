# Trader Behavior vs Market Sentiment  
**Junior Data Scientist – Trader Behavior Insights**

## Objective  
The objective of this analysis is to study how **Bitcoin market sentiment (Fear & Greed Index)** influences **trader performance, risk-taking behavior, and efficiency** using historical Hyperliquid trade data. The goal is to uncover actionable behavioral patterns that can inform smarter trading and risk-management strategies.

---

## Data Sources  
- **Bitcoin Market Sentiment Dataset**
  - Daily Fear & Greed classifications (Fear, Greed, Extreme Fear, Extreme Greed, Neutral)
- **Hyperliquid Historical Trader Data**
  - Trade-level data including account, execution price, position size, direction, and realized PnL

---

## Methodology  

### 1. Data Preparation
- Cleaned and aligned timestamps between trades and sentiment data
- Merged datasets on trading date
- Handled missing and invalid timestamps defensively

### 2. Feature Engineering
- Profitability indicator (`is_profitable`)
- Absolute PnL as a proxy for volatility
- Risk exposure approximated using position size (USD)
- Risk-adjusted return metric: `PnL / Risk`
- Extreme sentiment regime flag

### 3. Analysis Layers
- Performance vs sentiment
- Risk-taking behavior vs sentiment
- Risk-adjusted performance comparison
- Extreme sentiment stress testing
- Trader-level behavioral segmentation

---

## Key Findings  

- **Extreme Greed regimes generate the highest raw and risk-adjusted returns**, indicating that strong bullish conviction translates into profitable opportunities.
- **Fear regimes exhibit high risk exposure but poor efficiency**, suggesting emotional or forced trading behavior.
- **Extreme sentiment periods show higher profitability with lower average risk**, implying more selective and disciplined trades.
- **Risk-adjusted returns differ significantly from raw PnL rankings**, highlighting the importance of efficiency over aggressiveness.
- **Trader segmentation reveals behavioral alpha**: consistently profitable traders adapt risk exposure better across sentiment regimes than losing traders.

---

## Business Implications  

- Trading systems can benefit from **sentiment-aware risk controls**, tightening exposure during Fear and loosening selectively during Extreme Greed.
- Risk-adjusted metrics should complement raw PnL when evaluating trader performance.
- Behavioral segmentation enables targeted monitoring of high-risk trader archetypes.
- Extreme sentiment detection can be used as a **regime signal** for adaptive strategies.

---

## Limitations & Future Work  

- Leverage data was not explicitly available; risk exposure was approximated using position size.
- Future work could incorporate:
  - Time-based performance decay
  - Symbol-specific analysis
  - Real-time sentiment integration
  - Trader adaptation over time

---

## Conclusion  

This analysis demonstrates that market sentiment significantly impacts trader behavior, risk efficiency, and outcomes. Incorporating sentiment-aware analytics can materially improve trading intelligence and risk management in crypto markets.
