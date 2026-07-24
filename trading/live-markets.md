# Live Markets

Rocky currently supports both perpetual and spot markets.

## Perpetual markets

| Market   | Quote / Settlement Asset | Maximum Leverage |
| -------- | ------------------------ | ---------------- |
| BTC-PERP | CUSD                     | Up to 100x       |
| ETH-PERP | CUSD                     | Up to 100x       |
| CC-PERP  | CUSD                     | Up to 100x       |

Maximum leverage is a market limit, not a recommendation. The leverage available for an individual order may depend on market parameters, position size, liquidity, and risk controls.

## Spot markets

| Market    | Base Asset | Quote Asset |
| --------- | ---------- | ----------- |
| CBTC/CUSD | cBTC       | CUSD        |
| cETH/CUSD | cETH       | CUSD        |
| CC/CUSD   | CC         | CUSD        |
| cETH/CBTC | cETH       | CBTC        |

Spot markets exchange one asset directly for another and do not use perpetual funding or leveraged position mechanics.

{% hint style="info" %}
**Live-market notice**

Markets can be added, paused, or updated. Always check the [live trading interface](https://app.rocky.exchange/trade) for current availability and specifications.
{% endhint %}
