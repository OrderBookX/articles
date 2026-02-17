# How to Use Futures Grid Bot — Reading the Dashboard

Once your grid bot is running, the dashboard becomes your primary interface for monitoring performance and making decisions. Understanding what each metric means — and which combinations signal action — turns raw numbers into actionable intelligence.

## Key Dashboard Metrics

Grid profit is the cumulative realized gain from completed grid cycles. This number only increases while the bot is actively trading. Every buy-sell completion adds to it. When the bot pauses because price left the range, grid profit freezes at its current level.

## Unrealized PnL

Unrealized PnL shows the current profit or loss on your open position. If the bot is long and price has dropped since your last fill, unrealized PnL is negative. If price has risen, it's positive. This number fluctuates in real time with market movement. It represents money you haven't yet locked in — it could improve or worsen before you close the bot.

## Total PnL

Total PnL is the sum of grid profit and unrealized PnL. This is the number that tells you how you're actually doing. A bot with $100 grid profit and negative $150 unrealized PnL has a total PnL of negative $50. If you closed the bot right now, you'd realize a net loss despite the positive grid profit.

### Bot Status

Bot status tells you whether the bot is actively trading, paused because price exited the range, or stopped. A paused bot is holding a position but not placing new orders. This is a critical signal — if the bot has been paused for hours or days, the market has moved away from your range. You need to decide: wait for return, or stop and redeploy.

### Margin Usage

Margin usage shows how much of your allocated margin is currently being used. As more grid levels fill, margin usage increases. If usage approaches 100%, the bot is near its capacity and liquidation risk rises. This metric provides early warning before problems become severe.

Grid activity during off-hours deserves attention too. Crypto trades 24/7, but volume and volatility vary by timezone. If your bot is most active during Asian session hours and nearly idle during your local daytime, that pattern tells you something about the pair's rhythm. You can use this insight to set ranges that specifically target the asset's most active oscillation windows, potentially improving cycle frequency without widening the range.

## Putting It All Together

Together, these five metrics give you everything needed to manage a running [futures grid bot](https://www.bitunix.com/register?vipCode=BITUNIXBONUS&utm_source=3rdparty&utm_medium=keywordlinks-article). Check them daily. On Bitunix, all metrics display in the bot section of your assets with clear formatting. Knowing [how to use futures grid bot](https://www.bitunix.com/register?vipCode=BITUNIXBONUS&utm_source=3rdparty&utm_medium=keywordlinks-article) dashboards effectively is as important as the initial setup. [Monitor your grids in real time on Bitunix](https://www.bitunix.com/register?vipCode=BITUNIXBONUS&utm_source=3rdparty&utm_medium=shillers-channel-article).
