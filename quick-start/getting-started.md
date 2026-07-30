# Getting Started

## Open the application

Visit the [Rocky trading application](https://app.rocky.exchange/trade).

Always verify the domain before connecting a wallet or approving a transaction:

```
https://app.rocky.exchange
```

## Supported wallets

Rocky currently supports four Canton wallet login methods:

| Wallet             | Access                              |
| ------------------ | ----------------------------------- |
| **Rocky Wallet**   | Rocky's native wallet experience    |
| **Loop Wallet**    | Connect an existing Loop account    |
| **Console Wallet** | Connect an existing Console account |
| **Send Wallet**    | Connect an existing Send account    |

To connect:

1. Open the Rocky application.
2. Select **Connect Wallet**.
3. Choose Rocky Wallet, Loop Wallet, Console Wallet, or Send Wallet.
4. Confirm that the wallet is connected to **Canton Mainnet**.
5. Review and approve the login request in the wallet.

Your connected wallet is used for account access and for authorizing deposits and withdrawals. Rocky will never ask you to share a recovery phrase, private key, or wallet password.

{% hint style="info" %}
**Wallet compatibility**

Supported wallets and connection requirements may be updated. Refer to the live connection window in the application for the current list.
{% endhint %}

## Before you trade

Make sure that:

* Your wallet is connected to Canton Mainnet.
* You hold a supported deposit asset in the connected wallet.
* You have deposited sufficient funds from the wallet into your Rocky trading account.
* The deposit has been credited and is visible as available trading balance.
* You understand the difference between spot and leveraged perpetual trading.
* You have reviewed the market's collateral, leverage, minimum size, and fee information in the application.

{% hint style="info" %}
**Wallet balance and trading balance are separate**

Connecting a wallet allows you to log in and authorize transactions, but it does not automatically make the assets in that wallet available for trading. Before placing a perpetual or spot order, you must deposit a supported asset into your Rocky trading account and wait for the deposit to be credited.
{% endhint %}

## Account and balance structure

Rocky separates the assets held in a connected wallet from the balances available inside the trading platform.

| Account or balance            | Purpose                                                                                                       |
| ----------------------------- | ------------------------------------------------------------------------------------------------------------- |
| **Connected wallet balance**  | Assets held in Rocky Wallet, Loop Wallet, Console Wallet, or Send Wallet before they are deposited into Rocky |
| **Available trading balance** | Deposited funds that are available for new perpetual or spot orders                                           |
| **Perpetuals equity**         | The value assigned to perpetual trading, including available collateral and position profit or loss           |
| **Margin in use**             | Collateral currently supporting open perpetual positions and orders                                           |
| **Spot free balance**         | Spot assets available to place new orders or withdraw                                                         |
| **Spot locked balance**       | Spot assets reserved by open limit orders                                                                     |
| **Withdrawable balance**      | Funds that are not locked in orders or required as position margin and can be withdrawn                       |

The main balance relationships are:

```
Connected wallet
    ↓ Deposit
Rocky trading account
    ├─ Perpetuals equity → Available margin + Margin in use
    └─ Spot balance      → Free balance + Locked balance
```

### How balances change

* **Deposit** - moves a supported asset from the connected wallet into the Rocky trading account.
* **Open a perpetual position** - allocates part of the available balance as margin.
* **Place a spot limit order** - moves the required spot balance from free to locked while the order remains open.
* **Cancel an open order** - releases the unused locked balance.
* **Close a perpetual position** - releases the remaining margin and realizes the position's profit or loss.
* **Complete a spot trade** - deducts the sold asset and credits the purchased asset.
* **Withdraw** - moves an eligible balance from the Rocky trading account back to the selected wallet.

Available balance, equity, and withdrawable balance may differ because open orders, margin requirements, unrealized profit or loss, and pending transactions affect how much capital can be used or withdrawn.
