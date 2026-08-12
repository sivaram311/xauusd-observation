# 02 — Hypothesis & Analysis Framework

## Core Hypothesis (User-Driven)
> Every single candle is predictable with direction and where it will move / how it will behave. They are always referenced to the untouched open or close from the candle in the recent past. And it follows the same pattern over and over again.

If true, this creates an edge for entries with stop distance of only **0.50 – 1.00** (price points).

## Definitions We Will Use

**Untouched Open / Close**  
A prior candle’s Open or Close price that has **not** been traded through (i.e. subsequent High has not gone above it, or subsequent Low has not gone below it) until the moment we examine a new candle. These are “virgin” levels.

**Reference**  
Current candle’s open, high, low, close, or path is observed relative to one or more of these untouched levels from the last N candles (we start with N=5–20 and expand).

**Predictability Claim**  
Direction of the current candle (and often the next few) can be anticipated by:
1. Proximity to the nearest untouched O or C
2. Whether price is approaching from above or below
3. How the previous candle left that level (rejection, acceptance, gap, etc.)
4. Repeating micro-patterns around these levels across sessions

## Analysis Method (Slow & Systematic)
1. Take a completed candle C_t
2. Scan backward for the nearest untouched Opens and Closes
3. Record:
   - Distance from C_t open to those levels
   - Whether C_t high/low interacted with them
   - Direction and range of C_t relative to the level
   - What happened on C_{t+1}, C_{t+2}
4. Look for repeating sequences (e.g. “return to prior close → rejection → continuation in original direction”)
5. Measure frequency of tight rejections (0.50–1.00 range around the level)
6. Expand from M5 → M15 → H1 → H4 while keeping the same rules

## Success Criteria for Edge
- High percentage of times price reacts (rejects or accelerates) within 0.50–1.00 of an untouched O/C
- Directional bias after reaction is consistent enough to risk only that small distance
- Pattern repeats across different sessions and volatility regimes

Next: concrete examples from the most recent data.
