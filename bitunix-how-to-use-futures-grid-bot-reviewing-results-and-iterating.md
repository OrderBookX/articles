# How to Use Futures Grid Bot — Reviewing Results and Iterating

The most valuable phase of grid trading isn't the setup or the monitoring — it's the review. After each grid bot completes its run (whether by hitting TP, triggering SL, or being manually stopped), the data it produces teaches you more than any guide ever could.

## Basic Performance Review

Start with the basics. What was the total PnL? Was the result profitable, breakeven, or a loss? How long did the bot run? What percentage return did it produce on the allocated margin? Compare this against simply holding the asset over the same period. If the grid didn't outperform a basic hold strategy, understand why.

## Deep Analysis

Then go deeper. How many grid cycles completed? This tells you how active the bot was. A high cycle count with low total profit suggests spacing was too tight and fees consumed most of the gains. A low cycle count with decent per-cycle profit suggests the range could have been tighter for more frequent trading.

### Maximum Drawdown

Look at the maximum drawdown. At what point was total PnL most negative? How close did you get to your SL? If the drawdown was severe but the bot eventually recovered, your range and leverage were adequate but the experience might justify more conservative settings for comfort. If the drawdown triggered SL, analyze whether the range was too narrow, leverage too high, or if an unexpected market event was the cause.

### Time Paused

Check whether the bot spent significant time paused. Extended pauses mean price was outside your range. Multiple long pauses suggest your range wasn't well-matched to the market. Compare your range against the actual high-low of the asset during the bot's runtime to see how accurate your initial range selection was.

## Building Your Trading Log

Document everything: date, pair, direction, range, grids, leverage, margin, TP/SL levels, runtime, total PnL, max drawdown, cycle count, and time spent paused. After ten grid runs, patterns will emerge. After twenty, you'll have a personalized playbook that reflects your own decision-making style and the market conditions you trade in.

Grid count also affects your psychological experience. A bot with 50 grids shows frequent small profits in the dashboard — which feels productive and reassuring. A bot with 10 grids shows infrequent larger profits — which can feel like nothing is happening between cycles. Neither is objectively better, but knowing your own temperament helps you choose a grid count that you'll actually let run without premature intervention.

This iterative process is [how to use futures grid bot](https://www.bitunix.com/register?vipCode=BITUNIXBONUS&utm_source=3rdparty&utm_medium=keywordlinks-article) tools to build genuine skill. The bot provides execution. The review provides education. On Bitunix, completed bot performance data is stored and accessible, supporting systematic [futures grid strategy](https://www.bitunix.com/register?vipCode=BITUNIXBONUS&utm_source=3rdparty&utm_medium=keywordlinks-article) improvement over time. [Review, refine, and relaunch on Bitunix](https://www.bitunix.com/register?vipCode=BITUNIXBONUS&utm_source=3rdparty&utm_medium=shillers-channel-article).
