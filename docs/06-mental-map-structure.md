# 06 — Mental Map Structure (v0.1)

## Purpose
A living, machine-readable map of previous-candle open and close reference levels for XAUUSD.

These levels form the "mental map" of touch zones and untouched (virgin) zones that price repeatedly references.

## File Location
`data/mental-map-v0.1.json`

## Structure Overview

### meta
Basic metadata about generation time, source and version.

### levels
Full list of tracked previous-candle references (open or close).

Each level contains:
- `id` — unique identifier
- `price`
- `type` — open | close
- `tf` — timeframe of origin
- `origin` — candle time
- `status` — virgin | touched | invalidated
- `first_touched`
- `age_bars`
- `confluence` — other timeframes that also have a level nearby
- `strength` — high / medium / low
- `notes`

### active_map
Ranked subset of the most relevant levels right now (proximity to current price + age + confluence + strength).

This is the practical working set for decision making.

### clusters
Groups of nearby levels that form shelves / zones.

## Current Focus (v0.1)
- Backbone from deep M15 history (from ~4 Aug)
- Dense recent M1 levels for fine structure
- Emphasis on currently relevant levels around the 4395–4420 area
- Key historical anchors kept for context

## Next Steps
1. Expand with systematic back-processing of more M1 history
2. Add automatic age and first-touch calculation
3. Add H1 confluence layer
4. Make the map updateable in near real-time from live ticks/bars
