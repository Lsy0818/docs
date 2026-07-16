# Funding & Wallet Operations

Rocky is accessed through supported self-custodial wallet connections. Asset availability and transfer flows depend on the connected wallet and the assets supported by that wallet.

## Receive assets

1. Open the receive function in your connected wallet.
2. Verify the selected asset and Canton Mainnet.
3. Copy the receiving Party ID, address, or other identifier shown by the wallet.
4. Send a small test amount when using a new route or counterparty.
5. Confirm the transfer before committing a larger amount.

## Send assets

1. Open the send function in your connected wallet.
2. Enter the recipient information.
3. Select the asset and amount.
4. Review the recipient, network, amount, and fee.
5. Approve the transfer in the wallet.

> **Finality warning**
>
> On-chain transfers may be irreversible. An incorrect recipient, asset, or network selection can result in permanent loss.

## If a balance does not update

- Confirm that the transaction was submitted on Canton Mainnet.
- Verify that the receiving wallet supports the asset.
- Check whether the wallet requires an incoming transfer offer to be accepted.
- Refresh the wallet and Rocky application after settlement.
- Use the transaction reference to check the status on an official Canton explorer where available.
