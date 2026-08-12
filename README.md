# XAUUSD Observation

Deep research into XAUUSD (Gold) candle behaviour, predictability of direction and movement based on references to recent **untouched opens and closes**, and identification of edges for tight stop-loss entries (0.50 – 1.00 points).

## Core Thesis
Every candle’s direction and subsequent path is heavily influenced by (and often predictable from) open/close levels of recent prior candles that have not yet been “touched” (traded through). These virgin O/C levels act as magnets, barriers, or decision points. Patterns repeat across timeframes. Understanding these correlations can allow entries with extremely tight risk (0.50–1.00 in price terms).

## Structure
- [01-symbol-basics.md](docs/01-symbol-basics.md) — Contract specs, current state, tick behaviour
- [02-hypothesis-and-framework.md](docs/02-hypothesis-and-framework.md) — Formal definition of “untouched” levels and analysis method
- [03-recent-observations.md](docs/03-recent-observations.md) — Concrete examples from live M5 / M15 / H1 data (Aug 11–12 2026)
- More files will be added as we dive deeper candle-by-candle and timeframe-by-timeframe.

## Data Source
Live data via the running `xauusd-mcp` (MT5) connector.

## Status
Research in progress — starting slowly with recent candles and expanding.
