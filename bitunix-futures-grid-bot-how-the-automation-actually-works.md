# Futures Grid Bot — How the Automation Actually Works

Futures Grid Bot — How the Automation Actually Works

A futures grid bot is software that automates a specific type of trading strategy: buying low and selling high within a defined price range, over and over again. It removes the need for manual order placement, emotional decision-making, and constant chart monitoring. But understanding what happens under the hood helps you configure it properly.


## The Setup Process

When you create a grid bot, you provide several inputs: a trading pair, a price range (minimum and maximum), the number of grids, a direction (long or short), leverage, and the margin you want to allocate. The bot takes these inputs and calculates evenly spaced price levels across your range using arithmetic spacing. It then places limit orders at each level.


## How Orders Execute

For a long grid, the bot places buy orders below the current price and sell orders above it, within the range. As price drops to a buy level, the order fills. When price bounces to the next sell level, that order fills too — completing one grid cycle and locking in a small profit. This happens independently at every grid level, so multiple cycles can run simultaneously.


## Range Exit Behavior

If price moves outside your defined range, the bot pauses. No new orders are placed. The bot holds its current position and waits. When price re-enters the range, trading resumes automatically. This pause behavior is important to understand because it means your range selection directly controls how active the bot is.

Each [futures grid bot](https://www.bitunix.com/register?vipCode=BITUNIXBONUS&utm_source=3rdparty&utm_medium=keywordlinks-article) on Bitunix operates from a dedicated bot account. When you create a strategy, your allocated margin transfers from your spot account to this isolated container. The bot trades, earns, or loses within that container only — your other positions and balances remain untouched. This isolation is critical when running multiple bots.

The bot also tracks several performance metrics in real time. Grid profit shows your accumulated realized gains from completed cycles. Unrealized PnL reflects the current value of your open position. Total PnL combines both for a complete picture. These metrics are essential for deciding when to let the bot continue and when to stop and reconfigure. On Bitunix, all three are visible in the bot dashboard, giving you the data you need without switching between screens.

You can run up to 200 grid strategies simultaneously on Bitunix, each independent. When you stop a bot, all open orders cancel, positions close at market, and remaining funds return to your spot account. The process is transparent and immediate. Understanding how a [futures grid strategy](https://www.bitunix.com/register?vipCode=BITUNIXBONUS&utm_source=3rdparty&utm_medium=keywordlinks-article) executes at this level helps you set better parameters and avoid surprises. If you want to see it in action, [launching a grid on Bitunix takes minutes](https://www.bitunix.com/register?vipCode=BITUNIXBONUS&utm_source=3rdparty&utm_medium=shillers-channel-article).
