# Product Architecture

Rocky's architecture combines a high-performance execution layer with Canton-native settlement.

## Execution layer

- **Matching engine** - processes eligible buy and sell orders.
- **Order book** - organizes market liquidity and supports market-maker participation.
- **Market-maker API** - provides programmatic access for qualified liquidity providers.
- **Risk engine** - monitors margin, exposure, and liquidation conditions.

## Canton settlement layer

- **Daml contracts** - represent financial rights, obligations, and state changes.
- **Margin and position workflows** - coordinate collateral and position updates.
- **Asset workflows** - handle supported asset movements and transaction approvals.
- **Atomic settlement** - coordinates linked actions so they complete together or do not complete.
- **Selective visibility** - shares transaction data only with the parties required for the workflow.

This separation allows execution to remain responsive while settlement retains Canton's privacy and workflow capabilities.
