# Trade Value System

The Value module provides a real-time lookup and comparison system for items, ensuring users can trade fairly and accurately.

## Key Features
- **Real-Time Item Search**: Check the latest values, demand, and rarity for any supported item.
- **Trade Evaluator**: Compare multiple items on both sides to immediately see the trade outcome.
- **Visual Clarity**: Uses custom icons to make trade summaries easy to read.

## Commands

### Prefix Commands (Standard Usage)
- `,[item name]`: Look up the current market value and stats for a specific item.
- `,[side A] for [side B]`: Compares two groups of items, providing a total value comparison and a Win/Loss/Fair outcome.

### Slash Commands (Management)
- `/enable-values [channel]`: Restricts the use of value commands to a specific channel.
- `/disable-values`: Completely disables the value lookup feature for your server.

## Evaluation Logic
- Compares the total estimated value of both sides to provide a quick verdict.
- Automatically accounts for necessary community taxes in its calculations.
