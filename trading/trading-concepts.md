# Trading Concepts

## Long and short

- **Long** - gains value when the market price rises and loses value when it falls.
- **Short** - gains value when the market price falls and loses value when it rises.

## Leverage

Leverage allows a trader to control a position larger than the margin committed.

For example, a 10x leveraged position uses 1 unit of margin to control 10 units of market exposure. This magnifies profit and loss and brings the liquidation price closer to the entry price.

Use leverage according to your own risk tolerance. The maximum permitted leverage should not be treated as a target.

## Order types

The order types available in Rocky are displayed in the order panel and may vary by product or market.

Common order types include:

- **Market order** - seeks immediate execution at the best available prices. The final execution price can differ from the price visible when the order is submitted.
- **Limit order** - executes only at the specified price or better. Execution is not guaranteed.
- **Conditional order** - activates after a defined trigger is reached, where supported.
- **Take-profit / stop-loss** - helps automate an exit at a target or risk threshold, where supported.

Always rely on the live order panel for currently supported order types.

## Mark price

The mark price is a reference price used for position valuation and liquidation checks. It is intended to reduce the impact of short-lived price dislocations or isolated trades.

Your unrealized profit and loss and liquidation status may be calculated using the mark price rather than the latest traded price.

## Funding

Funding payments help keep a perpetual market aligned with its underlying reference price.

- When the perpetual trades above the reference price, long positions may pay short positions.
- When it trades below the reference price, short positions may pay long positions.

Funding is exchanged between market participants according to the active market mechanism; it is not the same as a trading fee. Review the current funding rate and timing before holding a position through a funding event.

## Margin and liquidation

Margin supports an open leveraged position. If losses reduce available margin below the applicable maintenance requirement, the position may become eligible for liquidation.

Ways to reduce liquidation risk include:

- Using lower leverage.
- Reducing position size.
- Maintaining additional available margin.
- Monitoring the liquidation price.
- Using risk-management orders where available.

Liquidation controls are designed to protect market solvency, but they do not prevent user losses.
