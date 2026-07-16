# Live Markets

Rocky currently supports both perpetual and spot markets.

## Perpetual markets

| Market | Quote / Settlement Asset | Maximum Leverage |
| --- | --- | --- |
| BTC-PERP | USDC | Up to 100x |
| ETH-PERP | USDC | Up to 100x |
| CC-PERP | USDC | Up to 100x |

Maximum leverage is a market limit, not a recommendation. The leverage available for an individual order may depend on market parameters, position size, liquidity, and risk controls.

## Spot markets

| Market | Base Asset | Quote Asset |
| --- | --- | --- |
| cBTC/USDCx | cBTC | USDCx |
| cETH/USDCx | cETH | USDCx |

Spot markets exchange one asset directly for another and do not use perpetual funding or leveraged position mechanics.

> **Live-market notice**
>
> Markets can be added, paused, or updated. Always check the [live trading interface](https://app.rocky.exchange/trade) for current availability and specifications.
