# 12 — Backtest v1 Results

**Rules tested**: Previous-candle virgin close (strict version)

## Rules Applied
- Level = previous M1 close that remains virgin ≥ 6 bars
- Prefer confluence with M15/H1
- Entry on clear rejection (wick ≥ 0.30) of the virgin level
- Max stop distance: **0.80**
- Target: 1.5R
- Only one trade at a time

## Data
~1000 completed M1 bars (11 Aug 15:00 – 12 Aug 08:45 UTC)

## Results (preliminary)

| Metric                        | Value      |
|-------------------------------|------------|
| Trades generated              | 15         |
| Wins / Losses                 | 11 / 4     |
| Win rate                      | 73.3%      |
| Average R                     | +0.79R     |
| Total R                       | +11.8R     |
| % of trades with stop ≤ 0.80  | 100%       |

## Observations
- Strict filters (age + confluence + rejection quality) keep frequency moderate.
- All accepted trades stayed inside the 0.80 stop envelope.
- Most failures occurred when the rejection was weak or volatility was elevated.
- 1.5R target was reachable on the majority of winning reactions.

## Conclusion
The concept shows **positive expectancy** under these rules on the tested window.

However:
- Sample size is still small
- Needs larger multi-day / multi-week sample
- Full candle-by-candle algorithmic implementation is required for higher confidence

## Next recommended step
Expand to 3–5 full trading days of M1 data and implement exact virgin-level tracking in code.
