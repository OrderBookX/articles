# Futures Grid Bot — What Nobody Tells You About Grid Spacing

Everyone talks about range selection and leverage when setting up a futures grid bot. Almost nobody talks about grid spacing — and it's the parameter that most directly determines whether your bot makes money or just generates trading volume.

## What Grid Spacing Actually Is

Grid spacing is the distance between each price level inside your range. It's determined by two inputs: the width of your range and the number of grids. A $10,000 range with 20 grids creates $500 spacing. The same range with 50 grids creates $200 spacing. This difference changes everything about how the bot performs.

## Tight Spacing vs Wide Spacing

Tighter spacing (more grids) means the bot trades more frequently. Every small price wiggle triggers a cycle. This sounds appealing — more trades, more profits, right? Not necessarily. Each trade incurs a fee. If your grid spacing is $200 and the per-grid profit at your leverage is $3, but the round-trip fee is $2.50, your net profit per cycle is only $0.50. You're keeping 17% of the gross profit. The exchange keeps the rest.

Wider spacing (fewer grids) means fewer trades but larger profit per cycle. A $500 spacing might yield $8 per cycle with the same $2.50 fee, netting $5.50 — a 69% retention rate. The bot trades less often, but each trade is meaningfully profitable.

## Finding the Sweet Spot

The optimal spacing depends on three factors: your fee tier, the asset's typical intraday volatility, and your leverage. Lower fees let you use tighter spacing profitably. Higher intraday volatility means tighter spacing gets triggered more often. Higher leverage amplifies per-grid profit, making tighter spacing viable even with moderate fees.

### A Practical Calculation

Here's a practical approach: calculate your per-grid profit at your chosen leverage and spacing, subtract the round-trip fee, and check if the net profit justifies the capital allocation. If net profit per cycle is less than 0.5% of per-grid margin, your spacing is probably too tight.

## The Fee Tier Feedback Loop

One more consideration: as your fee tier improves through higher trading volume, tighter spacing becomes more viable. A VIP trader paying 0.02% per side can profitably run grids that would be unprofitable for a standard-tier trader paying 0.05%. This creates a feedback loop — successful grid trading generates volume that improves your fee tier, which in turn makes your grids more profitable. Factor your current tier into your spacing calculation and recalculate as your tier upgrades.

On Bitunix, the [futures grid bot](https://www.bitunix.com/register?vipCode=BITUNIXBONUS&utm_source=3rdparty&utm_medium=keywordlinks-article) supports 2 to 200 grids with arithmetic spacing. Combined with competitive fee tiers that improve as your volume grows, you have the flexibility to find the spacing sweet spot for your [futures grid strategy](https://www.bitunix.com/register?vipCode=BITUNIXBONUS&utm_source=3rdparty&utm_medium=keywordlinks-article). Test different grid counts on small capital before scaling up. [Optimize your grid spacing on Bitunix](https://www.bitunix.com/register?vipCode=BITUNIXBONUS&utm_source=3rdparty&utm_medium=shillers-channel-article).
