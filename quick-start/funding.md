# Funding Your Rocky Trading Account

Rocky is accessed through supported wallet connections, but perpetual and spot orders use funds deposited into the user's Rocky trading account.

The basic fund flow is:

```
Connected wallet → Rocky trading account → Perpetual margin or spot trading balance
```

## Deposit funds

1. Connect Rocky Wallet, Loop Wallet, Console Wallet, or Send Wallet.
2. Confirm that the selected wallet account is connected to Canton Mainnet.
3. Open the deposit or funding section in Rocky.
4. Select a supported deposit asset.
5. Enter the amount you want to transfer to your Rocky trading account.
6. Review the asset, amount, destination, and any applicable fee.
7. Approve the deposit request through the connected wallet.
8. Wait for the transaction to complete and the amount to appear as available trading balance.

Do not place a perpetual or spot order until the deposit is shown as available balance in Rocky. A completed wallet transfer and a credited trading balance may not appear at exactly the same time.

## Withdraw funds

1. Open the withdrawal section in Rocky.
2. Select a supported asset and enter the withdrawal amount.
3. Confirm the destination wallet and review any applicable fee.
4. Submit the withdrawal request.
5. Wait for the withdrawal to complete and verify the updated balance in the receiving wallet.

{% hint style="danger" %}
**Finality warning**

Deposits and withdrawals may involve irreversible on-chain transfers. An incorrect wallet account, asset, destination, or network selection can result in permanent loss.
{% endhint %}

## If a deposit does not appear

* Confirm that the transaction was submitted on Canton Mainnet.
* Verify that the asset is currently supported for deposits.
* Confirm that the deposit was sent through the funding workflow displayed in Rocky.
* Check the transaction status in the connected wallet.
* Refresh the Rocky application after the transaction has settled.
* Use the transaction reference to check the status on an official Canton explorer where available.
* Contact official Rocky support and provide the transaction reference if the deposit remains uncredited.
