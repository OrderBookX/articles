# Futures Grid Trading Bot — Understanding Grid Profit vs Total PnL

Futures Grid Trading Bot — Understanding Grid Profit vs Total PnL

When monitoring a running grid bot, two numbers compete for your attention: grid profit and total PnL. They measure different things, can send opposite signals, and confusing them leads to bad decisions.


## Grid Profit Explained

Grid profit is the sum of realized gains from completed buy-sell cycles. Every time the bot buys at one grid level and sells at the next, that locked-in profit adds to this number. Grid profit only increases as long as the bot is actively completing cycles. It never goes down on its own.


## Total PnL: The Full Picture

Total PnL tells the complete story. It combines realized grid profit with unrealized profit or loss from the current open position. If the market has moved against your direction, the open position shows a loss that may offset or exceed your grid profits.


## When They Conflict

Here's where it gets tricky. A bot can show $150 in grid profit — which looks great — while sitting on $200 in unrealized loss from the open position. Total PnL is actually negative $50. If you close the bot at this point, you walk away with a net loss despite the encouraging grid profit number.

This happens commonly in trending markets. The bot keeps completing grid cycles (generating grid profit) while accumulating directional exposure against the trend (creating unrealized loss). The grid profit makes it feel like the bot is working. The total PnL tells you it's actually losing.

The reverse can also happen. After a drawdown, price may reverse toward your range, reducing the unrealized loss. If you wait, total PnL can recover and turn positive as the open position moves back in your favor and more grid cycles complete.

The psychological element is worth addressing too. Watching grid profit climb while total PnL fluctuates can be confusing and stressful. New grid operators often panic and close bots prematurely during temporary drawdowns that would have recovered. Having clear TP/SL settings removes this emotion from the equation. The bot continues executing until it reaches your predefined outcome — either profit target or loss limit. You made the decision when you were rational, not when you were watching price drop.

Understanding this distinction is essential for any [futures grid trading bot](https://www.bitunix.com/register?vipCode=BITUNIXBONUS&utm_source=3rdparty&utm_medium=keywordlinks-article) operator. Never make stop or hold decisions based on grid profit alone. Always check total PnL for the complete picture. On Bitunix, both metrics are visible in the bot dashboard, giving you clear [futures grid trading](https://www.bitunix.com/register?vipCode=BITUNIXBONUS&utm_source=3rdparty&utm_medium=keywordlinks-article) visibility at a glance. [Track your real performance on Bitunix](https://www.bitunix.com/register?vipCode=BITUNIXBONUS&utm_source=3rdparty&utm_medium=shillers-channel-article).
