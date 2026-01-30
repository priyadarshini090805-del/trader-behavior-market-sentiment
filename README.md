## Trader Behavior vs Market Sentiment

### Objective
Analyze how trader performance varies across Fear & Greed market regimes.

### Data
- Hyperliquid trades (211k+ rows)
- Fear & Greed Index (daily sentiment)

### Methodology
- Merge trades with sentiment by date
- Compute PnL, win-rate, risk exposure
- Compare sentiment-tagged vs baseline trades

### Key Findings
- Sentiment-tagged trades show higher avg PnL
- Extreme Greed has the strongest risk-adjusted returns
- Extreme Fear shows poorest performance

### Tech Stack
Python, Pandas, NumPy
